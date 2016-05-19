Ansible Role for PHP
====================

[![Build Status](https://travis-ci.org/pantarei/ansible-role-php.svg?branch=master)](https://travis-ci.org/pantarei/ansible-role-php)
[![GitHub tag](https://img.shields.io/github/tag/pantarei/ansible-role-php.svg)](https://github.com/pantarei/ansible-role-php)
[![GitHub license](https://img.shields.io/github/license/pantarei/ansible-role-php.svg)](https://github.com/pantarei/ansible-role-php/blob/master/LICENSE)

Ansible Role for PHP Installation.

Requirements
------------

This role require Ansible 2.0 or higher.

This role was designed for Ubuntu Server 14.04 LTS.

Role Variables
--------------

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>parameter</th>
<th>required</th>
<th>default</th>
<th>choices</th>
<th>comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>php_date_timezone</td>
<td>yes</td>
<td>Etc/UTC</td>
<td></td>
<td>The default timezone used by all date/time functions.</td>
</tr>
<tr class="even">
<td>php_display_errors</td>
<td>yes</td>
<td>Off</td>
<td></td>
<td>This determines whether errors should be printed to the screen as part of the output or if they should be hidden from the user.</td>
</tr>
<tr class="odd">
<td>php_display_startup_errors</td>
<td>yes</td>
<td>Off</td>
<td></td>
<td>Even when display_errors is on, errors that occur during PHP's startup sequence are not displayed.</td>
</tr>
<tr class="even">
<td>php_error_reporting</td>
<td>yes</td>
<td>E_ALL &amp; ~E_DEPRECATED &amp; ~E_STRICT</td>
<td></td>
<td>Set the error reporting level.</td>
</tr>
<tr class="odd">
<td>php_html_errors</td>
<td>yes</td>
<td>On</td>
<td></td>
<td>Turn off HTML tags in error messages.</td>
</tr>
<tr class="even">
<td>php_ignore_repeated_errors</td>
<td>yes</td>
<td>Off</td>
<td></td>
<td>Do not log repeated messages.</td>
</tr>
<tr class="odd">
<td>php_ignore_repeated_source</td>
<td>yes</td>
<td>Off</td>
<td></td>
<td>Ignore source of message when ignoring repeated messages.</td>
</tr>
<tr class="even">
<td>php_log_errors</td>
<td>yes</td>
<td>On</td>
<td></td>
<td>Tells whether script error messages should be logged to the server's error log or error_log.</td>
</tr>
<tr class="odd">
<td>php_max_execution_time</td>
<td>yes</td>
<td>30</td>
<td></td>
<td>This sets the maximum time in seconds a script is allowed to run before it is terminated by the parser.</td>
</tr>
<tr class="even">
<td>php_max_input_time</td>
<td>yes</td>
<td>60</td>
<td></td>
<td>This sets the maximum time in seconds a script is allowed to parse input data, like POST and GET.</td>
</tr>
<tr class="odd">
<td>php_memory_limit</td>
<td>yes</td>
<td>-1</td>
<td></td>
<td>This sets the maximum amount of memory in bytes that a script is allowed to allocate.</td>
</tr>
<tr class="even">
<td>php_post_max_size</td>
<td>yes</td>
<td>32M</td>
<td></td>
<td>Sets max size of post data allowed.</td>
</tr>
<tr class="odd">
<td>php_report_memleaks</td>
<td>yes</td>
<td>On</td>
<td></td>
<td>If this parameter is set to On (the default), this parameter will show a report of memory leaks detected by the Zend memory manager.</td>
</tr>
<tr class="even">
<td>php_session_save_path</td>
<td>yes</td>
<td>/tmp</td>
<td></td>
<td>Defines the argument which is passed to the save handler.</td>
</tr>
<tr class="odd">
<td>php_short_open_tag</td>
<td>yes</td>
<td>Off</td>
<td></td>
<td>Tells PHP whether the short form (&lt;? ?&gt;) of PHP's open tag should be allowed.</td>
</tr>
<tr class="even">
<td>php_track_errors</td>
<td>yes</td>
<td>Off</td>
<td></td>
<td>If enabled, the last error message will always be present in the variable $php_errormsg.</td>
</tr>
<tr class="odd">
<td>php_upload_max_filesize</td>
<td>yes</td>
<td>32M</td>
<td></td>
<td>The maximum size of an uploaded file.</td>
</tr>
<tr class="even">
<td>php_upload_tmp_dir</td>
<td>yes</td>
<td>/tmp</td>
<td></td>
<td>The temporary directory used for storing files when doing file upload.</td>
</tr>
</tbody>
</table>

Dependencies
------------

No additional role dependencies.

Example Playbook
----------------

    - hosts: all
      roles:
        - role: hswong3i.php

License
-------

-   Code released under [MIT](https://github.com/pantarei/ansible-role-php/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <a href="https://twitter.com/hswong3i" class="uri" class="uri">https://twitter.com/hswong3i</a>
    -   <a href="https://github.com/hswong3i" class="uri" class="uri">https://github.com/hswong3i</a>


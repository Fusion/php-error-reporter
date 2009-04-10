This is a sub-project that I extracted from the PHP Framework I called 'Lenses' (http://github.com/Fusion/lenses/tree)
This library can be used to display very verbose error reports, including stack traces, variables states, etc.
You may also ask the library to notify you when an error condition arises.
It will try to send you an email and if it fails will ask your users to report the error to you.
Of course you can modify this behaviour.



LICENSE:
========

See LICENSE.txt



USING THIS PROJECT:
===================

How to include this file is up to you. When used in the Lenses framework, it is included in the main index.php file, in the router class:

include('libs/error_reporter.php');

PHP can then be instructed to use this library for all kind of error reporting as follows:

register_shutdown_function('handleShutdown');
set_error_handler("displayErrorScreen");
set_exception_handler("displayExceptionScreen")

From now on, if a problem occurs, you should get very specific reports.


SETUP:
======

All you need to do is include error_reporter.php found in libs/



HELP!
=====

A support community for everything VoilaWeb-related (that's my company) including open-source projects is available at:
http://getsatisfaction.com/voilaweb
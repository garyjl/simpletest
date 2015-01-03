SimpleTest
==========

You probably got this package from:

    http://simpletest.org/en/download.html

If there is no licence agreement with this package please download
a version from the location above. You must read and accept that
licence to use this software. The file is titled simply LICENSE.

What is it? It's a framework for unit testing, web site testing and
mock objects for PHP 5.0.5+.

If you have used JUnit, you will find this PHP unit testing version very
similar. Also included is a mock objects and server stubs generator.
The stubs can have return values set for different arguments, can have
sequences set also by arguments and can return items by reference.
The mocks inherit all of this functionality and can also have
expectations set, again in sequences and for different arguments.

A web tester similar in concept to JWebUnit is also included. There is no
JavaScript or tables support, but forms, authentication, cookies and
frames are handled.

You can see a release schedule at http://simpletest.org/en/overview.html
which is also copied to the documentation folder with this release.
A full PHPDocumenter API documentation exists at
http://simpletest.org/api/.

The user interface is minimal in the extreme, but a lot of information 
flows from the test suite. After version 1.0 we will release a better 
web UI, but we are leaving XUL and GTK versions to volunteers as 
everybody has their own opinion on a good GUI, and we don't want to 
discourage development by shipping one with the toolkit. You can 
download an Eclipse plug-in separately. 

The unit tests for SimpleTest itself can be run here:

    test/unit_tests.php

And tests involving live network connections as well are here:

    test/all_tests.php

The full tests will typically overrun the 8Mb limit often allowed
to a PHP process. A workaround is to run the tests on the command
with a custom php.ini file or with the switch -dmemory_limit=-1
if you do not have access to your server version.


Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist garyjl/simpletest "*"
```

or add

```
"garyjl/simpletest": "*"
```

to the require section of your `composer.json` file.

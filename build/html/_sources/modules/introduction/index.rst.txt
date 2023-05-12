Introduction to Behat
=======================

Behat is an open source Behavior Driven Development framework for PHP 5.3+.

Behat is a tool to close the Behavior Driven Development (BDD) communication loop.

BDD is a methodology for developing software through continuous example-based communication between developers and a business, which this application supports.

This communication happens in a form that both the business and developers can clearly understand.

It is written in a special format called Gherkin.

COMMANDS IN BEHAT

To install behat with the help of composer

$ php composer.phar require --dev behat/behat

To initialize the feature suite structure inside your project, run:

$ behat --init

To view the version of the behat tool used, call:

$ behat -V

To execute behat

$ vendor/bin/behat

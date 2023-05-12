INTRODUCTION TO BEHAT
========================

Behat is an open source Behavior Driven Development framework for PHP 5.3+.

Behat is a tool to close the Behavior Driven Development (BDD) communication loop.

.. image:: images/image2.jpg


BDD is a methodology for developing software through continuous example-based communication between developers and a business, which this application supports.

This communication happens in a form that both the business and developers can clearly understand.

It is written in a special format called Gherkin.

**COMMANDS IN BEHAT**

To install behat with the help of composer

.. code-block:: bash

    $ php composer.phar require --dev behat/behat

To initialize the feature suite structure inside your project, run:

.. code-block:: bash

    $ behat --init

To view the version of the behat tool used, call:

.. code-block:: bash

    $ behat -V

To execute behat

.. code-block:: bash

    $ vendor/bin/behat

Array and Loops
==================


Declaring an array
---------------------

In PHP, the array() function is used to create an array:

.. code-block:: bash

    $array = [];

Example of an array

.. code-block:: bash

   <?php
   $cars = array("Volvo", "BMW", "Toyota");
   echo "I like " . $cars[0] . ", " . $cars[1] . " and " . $cars[2] . ".";
   ?>

Result : I like Volvo, BMW and Toyota.

Associative Array

Example of an associative array

.. code-block:: bash

   <?php
   $age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");
   echo "Peter is " . $age['Peter'] . " years old.";
   ?>

Result : Peter is 35 years old.

Looping over an array (Using an array)
-------------------------------------------

To loop through and print all the values of an array, you could use a foreach loop, like this:

.. code-block:: bash

   <?php
   $age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");

   foreach($age as $x => $x_value) {
   echo "Key=" . $x . ", Value=" . $x_value;
   echo "<br>";
   }
   ?>

Result : Key=Peter, Value=35

           Key=Ben, Value=37

           Key=Joe, Value=43




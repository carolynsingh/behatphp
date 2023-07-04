MySQL Connection using PDO
==============================

.. code-block:: bash

   sudo docker run --name mysql -d -p 3307:3306 --

   env="MYSQL_DATABASE=laravel" --

   env="MYSQL_ROOT_PASSWORD=Qwerty@321" --

   env="MYSQL_USER=test" --

   env="MYSQL_PASSWORD=Qwerty@321" mysql --bind_address=0.0.0.0

To start container :

.. code-block:: bash

   sudo docker start mysql

To execute :

.. code-block:: bash

   sudo docker exec -it mysql sh
   mysql -u root -p

Create database :

The CREATE DATABASE statement is used to create a database in MySQL.

.. code-block:: bash

   $sql = "CREATE DATABASE myDB";

Create table :

The CREATE TABLE statement is used to create a table in MySQL.

.. code-block:: bash

   $sql = "CREATE TABLE MyGuests (
   id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,
   firstname VARCHAR(30) NOT NULL,
   lastname VARCHAR(30) NOT NULL,
   email VARCHAR(50),
   reg_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
   )";

To insert data :

The INSERT INTO statement is used to add new records to a MySQL table:

.. code-block:: bash

   $sql = "INSERT INTO MyGuests (firstname, lastname, email)
   VALUES ('John', 'Doe', 'john@example.com')";

Select data :

The SELECT statement is used to select data from one or more tables:

.. code-block:: bash

   $sql = "SELECT column_name(s) FROM table_name";

or we can use the * character to select ALL columns from a table:

.. code-block:: bash

   $sql = "SELECT * FROM table_name";

Delete data :

The DELETE statement is used to delete records from a table:

.. code-block:: bash

   $sql = "DELETE FROM table_name WHERE some_column = some_value";

Construct PDO :

.. code-block:: bash

   try {

  $pdo = new PDO('mysql:host=127.0.0.1.3307;dbname=mydb', 'root', 'Qwerty@321');

  } catch (PDOException $e)

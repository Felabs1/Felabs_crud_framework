# Felabs_crud_framework
a Create Read Update Delete Framework Created to be used for easier create read update delete

# basic usage
download the code and import it in your project;
```php
include("crud.php");
// or
require("crud.php");
```
based on your coding practices. make sure the file location is linked well.


# Database Connection
```php
$crud = new Crud($server, $username, $password, $database)
```

# insert Data
```php
//create a variable like this 
$insert = $crud->insert_data($tablename, [
  "name" => $name,
  "age" => $age
]);
# in the associative array, the key values should be the same as the table columns in your mysql database 


```

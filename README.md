# Felabs crud framework
a Create Read Update Delete Framework Created to be used for easier create read update delete

# basic usage
download the code and import it in your project;
```php
include("crud.php");
// or
require("crud.php");
// or
include_once("crud.php");
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

# fetch data
```php
//create a variable like this
$crud->fetch_data("SELECT * FROM tablename");

//other functions you can use
count();
json_encode(); // and many more

```

# update data
```php
//do like this
$update = $crud->update_data($tablename, [
  "name" => $name, //fields to update
  "age" => $age
], [
  "id" => $id // conditions criteria
])

# the keys table should ne the same as the names you gave the columns in your table

```
# delete data
```php
// do this way
$delete = $crud->delete_data("DELETE FROM tablename WHERE id = '1'");
```
this project is for beginers but experts can also check on it. it's 100% php

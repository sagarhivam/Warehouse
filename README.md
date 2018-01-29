To run the code on your environment setup 

Please change the database details in includes/connection.php and includes/settings.ini file

If you are using sql server authentication, change the parameters username and password  in settings.ini file

Or if you are using Windows authentication, set those parameters to blank like
username=''
passwotrd=''

and remove those parameters from connection.php

Example:-

$connectionInfo = array( "Database"=>$INI['dbname'] , "UID"=>$INI['username'], "PWD"=>$INI['password']);

to

$connectionInfo = array( "Database"=>$INI['dbname']);

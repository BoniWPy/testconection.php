# testconection.php
#cek connection from webapps server to offsite database server


<?php
$link = mysqli_connect("your host/ip database server", "databaseUser", "Password", "DatabseName");

if (!$link) {
    echo "Error: Unable to connect to MySQL." . PHP_EOL;
    echo "Debugging errno: " . mysqli_connect_errno() . PHP_EOL;
    echo "Debugging error: " . mysqli_connect_error() . PHP_EOL;
    exit;
}

echo "Success OM >> OM telolet OMMMM..... (Tetttttt...tetttt...)" . PHP_EOL;
echo "Host information: " . mysqli_get_host_info($link) . PHP_EOL;

mysqli_close($link);
?>

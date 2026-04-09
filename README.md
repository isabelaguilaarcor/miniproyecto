<?php
// 1. Configuración de la conexión
$servidor = "localhost";
$usuario  = "root";
$password = ""; // Cambia esto si tienes contraseña en MySQL
$base_datos = "nombre_de_tu_base_de_datos";

$conexion = new mysqli($servidor, $usuario, $password, $base_datos);

// Verificar conexión
if ($conexion->connect_error) {
    die("Error de conexión: " . $conexion->connect_error);
}

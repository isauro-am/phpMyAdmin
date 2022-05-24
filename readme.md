# Docker phpMyAdmin
## Levantar un servicio local de phpMyAdmin

Para levantar el servicio de docker con phpMyAdmin para acceder a una base de datos remota.


- Definir el HOST dentro del archivo .env
- Proporcionar los datos de Conexion ( Usuario, Contraseña )
- Levantar el contenedor

Para levantar el servicio dentro de la carpeta donde esta el archivo .env y docker-compose.yml ejecutamos
```sh
docker-compose up -d
```

Si las credenciales de acceso son correctas asi como nuestro HOST es accesible, se puede acceder al servicio de phpMyadmin
Mediante el navegador bajo la ruta localhost:8080

### Alternativa

Si no se desea hacer una instalacion en el servidor remoto de phpMyAdmin, se puede colocar en el Adminer, que es un gestor de base de datos similar a phpMyAdmin pero este consta unicamente de un archivo PHP

```sh 
wget https://github.com/vrana/adminer/releases/download/v4.8.1/adminer-4.8.1.php

# https://www.adminer.org/
```
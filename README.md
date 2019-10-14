# SGD_CHILE
SISTEMA DE GESTION DOCUMENTAL - CHILE

[![License](https://img.shields.io/badge/licence-Apache%202.0-brightgreen.svg?style=flat)](LICENSE)
[![Build Status](https://travis-ci.org/Samsung/TizenRT.svg?branch=master)](https://travis-ci.org/Samsung/TizenRT)

## Contenido

> [Requisitos](#requisitos)  
> [Instalación](#instalación)  
> [Configuración](#configuración)  

## Requisitos

```bash
======================================================================================
Sistema Operativo	• Linux (CentOS7+) (64 bits)
Hardware		• 2 x Intel Xeon 3.0 GHz 
			• 8 GB RAM (+1GB cada 1.000 Usuarios Activos)
			• 1 TB HD (+1TB por cada 100.000 Usuarios)
Servidor Web		• Apache Web Server 2.4.x 
			• PHP 5.4+
Software adicional	• Certificado SSL
Bases de datos		• MySQL 7+
======================================================================================
```

```bash
======================================================================================
- Jquery	https://jquery.com/

- Bootstrap	https://getbootstrap.com/

- AdminLTE	https://adminlte.io/themes/AdminLTE/index2.html

- Jquery.Datatable	https://datatables.net/

- Jquery.LiveQuery	https://plugins.jquery.com/livequery/

- Font Awesome	https://fontawesome.com/

- Select2	https://select2.org/

- reCAPTCHA	https://www.google.com/recaptcha/intro/v3.html

- Moment	https://momentjs.com/
======================================================================================
```


## Instalación
Para instalar Apache, se debe ejecutar el siguiente comando:
```bash
yum install httpd
```

Luego de instalar Apache, se debe correr el demonio con el siguiente comando:
```bash
systemctl start httpd
```

Para habilitar el servicio de Apache con el inicio del sistema, se debe ejecutar el siguiente comando:
```bash
systemctl enable httpd
```

Para instalar PHP con las librerías, se debe ejecutar el siguiente comando:
```bash
yum install php php-mcrypt php-cli php-gd php-curl php-mysql php-ldap php-zip php-fileinfo
```

Para instalar MySQL se debe ejecutar el siguiente comando:
```bash
yum install mysql
```

Clonar el repositorio:
```bash
git clone https://github.com/compuvalpo/sgd_chile.git
```


## Configuración
- Renombrar el archivo /sys/Config.php.example a /sys/Config.php

- En Configurar ENVIROMENT y Base de Datos en archivo /sys/Config.php

- Crear directorios, dar permisos 775 y dueño el usuario apache:
```bash
	archivos/
	archivos/documentos
	app/views/templates_c/
	tmp/cache/
	tmp/logs 
```
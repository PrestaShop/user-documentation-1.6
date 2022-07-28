# Instalación de PrestaShop utilizando la secuencia de línea de comandos

Desde la versión 1.5.4, PrestaShop cuenta con un instalador de línea de comandos.

## ¿Qué es esto? <a href="#instalaciondeprestashoputilizandolasecuenciadelineadecomandos-queesesto" id="instalaciondeprestashoputilizandolasecuenciadelineadecomandos-queesesto"></a>

Este instalador especial hace posible la instalación de PrestaShop sin la necesidad de utilizar un navegador web: simplemente coloque el contenido del archivo zip en su servidor web, y podrá instalar PrestaShop a través de su interfaz de línea de comandos (CLI). Puede utilizar cualquier software CLI para interactuar con los comandos del servidor: Bash, Windows PowerShell, X Terminal OS, PuTTY, etc.

El interés de tener un instalador CLI además de la instalación típica (a través del navegador) es el de poder satisfacer las expectativas de algunos usuarios avanzados, ya que tienden a proporcionar un medio más conciso y potente para controlar algún programa o sistema operativo.

## ¿Cómo utilizarlo? <a href="#instalaciondeprestashoputilizandolasecuenciadelineadecomandos-comoutilizarlo" id="instalaciondeprestashoputilizandolasecuenciadelineadecomandos-comoutilizarlo"></a>

El instalador CLI es muy sencillo de utilizar: desde su terminal, diríjase a la carpeta `/install` (o `/install-dev`), e iniciar el script con este comando:

```
$ php index_cli.php
```

Al ejecutar este comando, se mostrarán las distintas opciones disponibles.

![](<../../.gitbook/assets/16779385 (2).png>)

Todas las opciones del instalador clásico están disponibles, con sus valores por defecto claramente indicados. Casi todos los valores se pueden dejar como están, porque pueden ser cambiados  más adelante desde el back-office de PrestaShop una vez finalice la instalación. Tenga en cuenta que el correo electrónico y la contraseña son los que se utilizan para crear la cuenta administrador del back-office de su tienda...

Para iniciar la instalación, sólo es necesario proporcionar un argumento. En realidad, es necesario proporcionar alguno más:

* **domain**. La ubicación en la que desea que aparezca su tienda.
* **db\_server**. La dirección del servidor de la base de datos.
* **db\_name**. El nombre de la base de datos que desea utilizar.
* **db\_user**. El nombre de usuario para la base de datos que desea utilizar.
* **db\_password**. La contraseña para el nombre de usuario de la base de datos que desea utilizar.

Por ejemplo:

```
$ php install_cli.php --domain=example.com --db_server=sql.example.com --db_name=prestashop --db_user=root --db_password=123456789
```

![](<../../.gitbook/assets/16779386 (2).png>)

Si además quiere puede establecer el valor `--email` a su propia dirección de correo electrónico. Un informe de la instalación a modo de resumen será enviado por correo al final de la instalación.

## Lista de argumentos <a href="#instalaciondeprestashoputilizandolasecuenciadelineadecomandos-listadeargumentos" id="instalaciondeprestashoputilizandolasecuenciadelineadecomandos-listadeargumentos"></a>

A continuación se presenta una lista de argumentos para index\_cli.php a partir de la versión 1.6:

| Nombre         | Valor por defecto                               | Descripción                                                             |
| -------------- | ----------------------------------------------- | ----------------------------------------------------------------------- |
| --step         | process                                         |                                                                         |
| --language     | en                                              | Código de idioma ISO                                                    |
| --timezone     | localhost                                       |                                                                         |
| --domain       | localhost                                       |                                                                         |
| --db\_server   | localhost                                       |                                                                         |
| --db\_user     | root                                            |                                                                         |
| --db\_password | (blank)                                         |                                                                         |
| --db\_name     | prestashop                                      |                                                                         |
| --db\_clear    | 1 (true)                                        | Eliminar tablas existentes                                              |
| --db\_create   | 0 (false)                                       | Crear la base de datos si no existe todavía                             |
| --prefix       | ps\_                                            |                                                                         |
| --engine       | InnoDB                                          | InnoDB/MyISAM                                                           |
| --name         | PrestaShop                                      | Nombre de la tienda                                                     |
| --activity     | 0                                               |                                                                         |
| --country      | fr                                              |                                                                         |
| --firstname    | John                                            |                                                                         |
| --lastname     | Doe                                             |                                                                         |
| --password     | 0123456789                                      |                                                                         |
| --email        | [pub@prestashop.com](mailto:pub@prestashop.com) |                                                                         |
| --license      | 0 (false)                                       | Mostrar licencia de PrestaShop                                          |
| --newsletter   | 1 (true)                                        | Suscribir administrador al boletín de noticias de PrestaShop            |
| --send\_email  | 1 (true)                                        | Enviar un correo electrónico al administrador después de la instalación |

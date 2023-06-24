# Configuración de PHPUnit en tu proyecto

A continuación, se detallan los pasos necesarios para configurar y utilizar PHPUnit en tu proyecto:

## Paso 1: Instalación de PHPUnit

Ejecuta el siguiente comando en la terminal para instalar PHPUnit en tu proyecto:

```bash
composer require --dev phpunit/phpunit ^9
```
## Paso 2: Configuración de la carga automática
Abre el archivo composer.json y agrega la siguiente sección al final del archivo:
```json
"autoload": {
    "classmap": [
        "src/"
    ]
}
```
Guarda el archivo composer.json después de realizar los cambios.
## Paso 3: Generar la carga automática optimizada
Ejecuta el siguiente comando en la terminal para generar la carga automática optimizada:

```bash
composer dump-autoload -o
```
## Paso 4: Ejecución de las pruebas
Ejecuta el siguiente comando en la terminal para ejecutar las pruebas utilizando PHPUnit:

```bash
./vendor/bin/phpunit test
```
Asegúrate de reemplazar "test" con la ubicación
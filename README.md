# Monolog 📝

Sends your logs to files, sockets, inboxes, databases and various web services.

Monolog sends your logs to files, sockets, inboxes, databases and various web services. Special handlers allow you to build advanced logging strategies. This library implements the [PSR-3](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-3-logger-interface.md) interface that you can type-hint against in your own libraries to keep a maximum of interoperability.

---

## English 🇬🇧

### 🚀 What the project does

Monolog is a comprehensive logging library for PHP. It allows you to send log messages to a wide variety of destinations (handlers), including:
- Files and sockets
- Databases (MongoDB, CouchDB, Redis, Elasticsearch, etc.)
- Email and messaging services (Slack, HipChat, etc.)
- Cloud services (AWS, Google Cloud, etc.)
- Browser consoles

### ✨ Why the project is useful

- **PSR-3 Compliance:** Fully compatible with the PHP Standard Recommendation for logger interfaces, ensuring interoperability.
- **Flexible Handling:** Stack multiple handlers to send logs to different locations based on severity levels.
- **Formatting & Processing:** Customize how logs are formatted (JSON, HTML, etc.) and enrich them with extra data using processors.
- **Robust:** Used by major frameworks like Symfony and Laravel.

### 🏁 How users can get started

#### Installation

Install the latest version with [Composer](https://getcomposer.org/):

```bash
composer require monolog/monolog
```

#### Basic Usage

Here is a basic setup to log to a file and to the output stream (e.g. stderr):

```php
<?php

use Monolog\Level;
use Monolog\Logger;
use Monolog\Handler\StreamHandler;

// create a log channel
$log = new Logger('name');
$log->pushHandler(new StreamHandler('path/to/your.log', Level::Warning));

// add records to the log
$log->warning('Foo');
$log->error('Bar');
```

For more documentation, see:
- [Usage Instructions](doc/01-usage.md)
- [Handlers, Formatters & Processors](doc/02-handlers-formatters-processors.md)

### ❓ Where users can get help

- **Documentation**: See the `doc/` directory for detailed guides.
    - [Utilities](doc/03-utilities.md)
    - [Extending Monolog](doc/04-extending.md)
- **Issues**: Report bugs or feature requests on the [GitHub Issue Tracker](https://github.com/Seldaek/monolog/issues).

### 👥 Who maintains and contributes

**Maintainer:**
- [Jordi Boggiano](https://github.com/Seldaek)

**Contributing:**
See [CONTRIBUTING.md](.github/CONTRIBUTING.md) (if available) or check the repository for contribution guidelines.

---

## Español 🇪🇸

### 🚀 Qué hace el proyecto

Monolog es una biblioteca de registro (logging) completa para PHP. Permite enviar mensajes de registro a una amplia variedad de destinos (handlers), incluyendo:
- Archivos y sockets
- Bases de datos (MongoDB, CouchDB, Redis, Elasticsearch, etc.)
- Servicios de correo electrónico y mensajería (Slack, HipChat, etc.)
- Servicios en la nube (AWS, Google Cloud, etc.)
- Consolas del navegador

### ✨ Por qué es útil

- **Cumplimiento PSR-3:** Totalmente compatible con la Recomendación Estándar de PHP para interfaces de registro, asegurando interoperabilidad.
- **Manejo Flexible:** Apila múltiples manejadores para enviar registros a diferentes ubicaciones según los niveles de severidad.
- **Formato y Procesamiento:** Personaliza cómo se formatean los registros (JSON, HTML, etc.) y enriquécelos con datos adicionales usando procesadores.
- **Robusto:** Utilizado por grandes frameworks como Symfony y Laravel.

### 🏁 Cómo empezar

#### Instalación

Instala la última versión con [Composer](https://getcomposer.org/):

```bash
composer require monolog/monolog
```

#### Uso Básico

Aquí hay una configuración básica para registrar en un archivo y en el flujo de salida (por ejemplo, stderr):

```php
<?php

use Monolog\Level;
use Monolog\Logger;
use Monolog\Handler\StreamHandler;

// crea un canal de registro
$log = new Logger('nombre');
$log->pushHandler(new StreamHandler('ruta/a/tu.log', Level::Warning));

// añade registros al log
$log->warning('Foo');
$log->error('Bar');
```

Para más documentación, consulta:
- [Instrucciones de Uso](doc/01-usage.md)
- [Handlers, Formatters & Processors](doc/02-handlers-formatters-processors.md)

### ❓ Dónde obtener ayuda

- **Documentación**: Consulta el directorio `doc/` para guías detalladas.
    - [Utilidades](doc/03-utilities.md)
    - [Extendiendo Monolog](doc/04-extending.md)
- **Problemas**: Reporta errores o solicita funciones en el [Rastreador de Problemas de GitHub](https://github.com/Seldaek/monolog/issues).

### 👥 Quién mantiene y contribuye

**Mantenedor:**
- [Jordi Boggiano](https://github.com/Seldaek)

**Contribución:**
Consulta las pautas de contribución en el repositorio.

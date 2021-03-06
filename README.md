# Work-in-out

#PRIMER HITO#

### Plataforma enfocada a los deportistas, híbrido entre red social y tablón de eventos. Proyecto relacionado con la asignatura DAI.

## Integrantes

* Jesús García Godoy

* Samuel Carmona Soria

* David Santiago Carrión

## Descripción

El proyecto consiste en una plataforma virtual pensada a modo de híbrido entre red social y tablón de eventos. La plataforma se centra en los deportistas y pretende abarcar todo su rango, desde principiantes a avanzados.
Entrando en detalle, la plataforma consistiría en un sitio web donde es necesario el registro, y en el cual se tiene acceso a un tablón de eventos donde los distintos usuarios puede tanto visualizar (y unirse) a los eventos ya creados por otros usuarios como también crear un evento nuevo, al cual los demás puedan unirse.

Cada evento especifica dentro de sí todos sus detalles y al tipo de público al que va dirigido, además de mostrar los participantes que asistirían y los comentarios que se han hecho al respecto sobre el mismo.
Debido a la naturaleza de la plataforma, orientada mayormente al campo abierto, se pretende hacer uso de integración con mapas, posibilitando así funcionalidades como ver rutas, compartirlas, etc...

Además , la plataforma actuará como una especia de red social, siendo capaz cada usuario de tener su red de amigos, así como de permanecer en contacto con estos por mensajería.

## Requisitos básicos

* Tablón de eventos

* Funciones propias de una red social(mensajería, comentarios, etc...)

* Gestión de rutas

* Organización por deportes

## Trabajo futuro

- Chat

- Versión móvil

- Creación de grupos

## Herramientas a usar

* Usaremos **Flask** como framework para la aplicación.

* **Python**, para la parte del servidor, así como funcionalidades de la web.

* **HTML5** y **CSS3** para la interfaz web.

* **MySQL**, para bases de datos de usuarios y eventos.

## Módulos

* **[Módulo 1, Jesús García Godoy](https://github.com/jesmorc/Proyecto-IV-modulo1)**: Este módulo se centrará en el servidor de bases de datos, el cual necesitaremos para almacenar los datos de la aplicación, como los usuarios, eventos, comentarios, etc...

* **[Módulo 2, David Santiago Carrión](https://github.com/dscdac/Proyecto-IV-modulo2)**: Este módulo se enfocará del front-end de la aplicación.

* **[Módulo 3, Samuel Carmona Soria](https://github.com/Samuc/Proyecto-IV-modulo3)**: Por último, este módulo se encargará de gestionar el servidor web que alojará la aplicación.

## Participación en el certamen de proyectos de libres organizado por la Oficina de Software Libre de la UGR

El proyecto ha sido inscrito en el certamen de proyectos libres de la UGR.

#SEGUNDO HITO#

#Integración Continua

Hemos usado Travis para la integración continua.

![travis1](http://i.imgur.com/61PhAWG.png)

#Fichero .travis.yml

Hemos especificado en el fichero **.travis-yml** las dependencias a instalar así como indicar que *nose* debe ejecutar los tests que existan.
```
language: python   

python:
  - "2.7" 

install:
   - sudo apt-get install libmysqlclient-dev
   - sudo apt-get install python-dev
   - pip install --upgrade pip
   - pip install MySQL-python
   - pip install Flask
   - pip install nose  

script:       # script para tests
   - nosetests

```

#Tests

Tras ejecutar los tests vemos en *travis* que funciona correctamente y se han pasado.

![travis2](http://i.imgur.com/0vSpiO8.png)

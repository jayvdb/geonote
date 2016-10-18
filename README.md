GEONOTE v1.5.0 (alpha)
======================

Web-based application for storage geodata

[DEMO](http://geonote.ru)


## Server-side 

Requirements:

- Django => 1.10.0
- PostgresSQL/PostGIS

Installation:
    
    $ git clone https://github.com/rendrom/geonote.git
    $ cd ./geonote
    $ virtualenv ./.env
    $ . ./.env/bin/activate
    $ pip install -r requirements.txt
    $ cp ./prj/local_settings.py.template ./prj/local_settings.py
    $ vim ./prj/local_settings.py #  edit database connection
    $ ./manage.py migrate
    $ ./manage.py runserver # go to http://localhost:8000

### Client-side

Requirements:
- [Nodejs](http://nodejs.org/)
- [npm](https://www.npmjs.org/)
- [grunt](http://gruntjs.com/)

Major library versions: 
- Angular 1.5.x
- Leaflet 0.7.7

Development:

    $ cd ./client
    $ npm install
    & grunt
    
## ToDo:

General:

- i18n
- documentations 
- tests, tests everywhere
- increase stability
- error handling

Server-side:

- refactoring
- simplify dynamic URLs
- extract Dynamit REST classes and methods
- support all spatial format import
- export data to various format
- plugin system (calculator)
- database tools (merge, clone)
- optimization for large dataset
- test memory with many dynamit-tables
- Python 3.x compatibility 

Client-side:

- switch to angular2 and typescript, webpack
- upgrade leaflet to 1.0.1 version
- make independent from the server-side
- create fake REST-service 
    
## Changelog:
* 19.10.2016 - django 1.8 to 1.10; angular 1.3 to 1.5

## Authors

Artemiy Doroshkov rendrom@gmail.com







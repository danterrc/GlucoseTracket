
PROYECTO DJANGO EXAMEN
======================

Un proyecto plantilla para Django 1.7
--------------------------------------

Antes de usar el proyecto tienes que hacer esto:

#. Crear tu entorno de trabajo
#. Instalar Django
#. Crear el nuevo proyecto usando la plantilla de django-examen
#. Instalar las dependencias adicionales

Creación del entorno de trabajo
==============================
Se crea asi un entorno de trabajo virtual una vez instalado virtualenvwrapper::

     $ mkproject django_projects/dirmod.asp?sid=&type=gen&mod=Core+Pages&gid=A6CD4967199A42D9B65B1B”. You will b

Instalación de DJANGO
=====================
Para la instalación de django es necesario que tenga instalado pip::
    
     $ sudo apt-get install python-pip
     $ pip install django==1.7

NOTA: La instalación de django se hara en su última versión sino lo pones la
version que quieres instalar.

Creacion de tu Proyecto
=======================
Para crear un nuevo proyecto Django llamado 'anime' usamos djangoforever.
Ejecute el siguiente comando::

     $ django-admin.py startproject --template=https://github.com/danterrc/djangoforever/archive/master.zip --extension=py,rst,html anime 

Instalación de Dependencias
===========================

En Desarrollo::

     $ pip install -r requirements/local.txt

Para Producción::
   
     $ pip install -r requirements.txt

Para generar modelos gráficos de tus aplicaciones
=================================================
Escribe el siguiente comando::
     $ python manage.py graph_models -a -g -o mi_modelo.png

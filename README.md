#camocat

##INTRODUCTION Catalogue of camouflage. Uses the following
technology stack:

1.  Python
2.  virtualenv
3.  Django
4.  mezzanine
5.  cartridge

##OVERVIEW OF SETUP

-   <http://cartridge.jupo.org/overview.html>
-   <http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create-deploy-python-django.html>

##STEPS TO CREATE

1.  `virtualenv camoenv`
2.  `source camoenv/bin/activate`
3.  `pip install -U cartridge`
4.  `pip install bleach`
5.  `mezzanine-project -a cartridge camocat`
6.  `cd camocat`
7.  `python manage.py createdb --noinput`
8.  `pip freeze &gt; requirements.txt`
9.  `python manage.py runserver`
10. <http://127.0.0.1:8000/> (`ctrl+c` to stop)
11. `deactivate`

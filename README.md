Django + MariaDB (MySQL) + Fig = Example
============================

This project is a simple example of a [Fig](http://orchardup.github.io/fig/)
project setup. It uses Django and MariaDB.

Running Requirements
====================

* [Fig](http://www.fig.sh/)
* [Docker](http://docker.io/)

These two requirements must be setup and are outside the scope of this readme. The links above are a good starting place.

Start Fig
=========

```bash
$ git clone https://github.com/jorge-3/fig-django-mariadb-example.git
$ cd fig-django-mariadb-example
$ fig up -d
$ fig run web python manage.py syncdb --noinput
```

Now browse to [http://localhost:8000](http://localhost:8000)

The Django server was started in auto-reload mode and fig shares the
current folder with the docker instance, so you can edit the python code
to see changes!

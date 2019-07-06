<!-- {% if not project_name %} -->

![Kickstart Coding Logo](./logo.png)

# Kickstart Coding: Django Project Starter


This is an example start project for [Kickstart Coding](http://kickstartcoding.com/)
Django projects.

It provides a solid foundation for building a Django project that's ready to
launch to Heroku or similar web-hosting service.


## Features

* Bootstrap 4: It's all set-up with Bootstrap 4 templates, and a few example
  pages.

* Log-in / sign-up: It includes a log-in and sign-up system ready-to-go.

* Custom user class: It features a custom user class that you can

* Heroku support: It's one `git push` away from publishing to the world

* Pipenv: It's set-up to use Pipfile

* Nice stuff:
    * `django-debug-toolbar` is installed and ready to go!
    * Separate `local` and `production` settings


## Who is this for

* This is for **new Python/Django programmers**, including **coding class
  students** who want a solid start for a Django project that uses SQLite when
  developing locally, and is ready to deploy Heroku provisioned Postgres
  database.

* The documentation assumes you already have fundamental Python, Django, Bash
  and Heroku knowledge. If you are new to Heroku, read our [Heroku Getting
  Started guide](http://github.com/kickstartcoding/heroku-getting-started/).

* The documentation *does not* explicitly support Windows. It assumes you use
  either **macOS** or **Ubuntu GNU/Linux**.

> This was original created for Kickstart Coding, the affordable,
> inclusive, and intensive coding course teaching cutting-edge Python /
> Django and JavaScript / React web development in Oakland, CA.
> [Learn more and enroll here.](http://kickstartcoding.com/?utm_source=github&utm_campaign=cheatsheets)


## Getting started

* Prereq: [You have Pipenv installed.
  ](https://github.com/kickstartcoding/pipenv-getting-started) You have Django
  admin installed globally (macOS type `pip3 install django`, Ubuntu GNU/Linux,
  type `sudo pip3 install django`)

1. Assuming `mycoolproject` is the name of your project, you should start a new
project using this template as follows:

    django-admin startproject --template=https://github.com/kickstartcoding/django-kcproject-starter/archive/master.zip mycoolproject


2. Go into the newly created project, and use `pipenv` to get your virtualenv
setup:

    cd mycoolproject
    pipenv shell
    pipenv install

3. Migrate to create the SQLite database:

    python manage.py migrate

4. Get the server running:

    python manage.py runserver

## Tour of files



    Diretory structure description below:

```python
[name_of_project]/
    - config/        
        - base.py          # Stores most settings
        - local.py         # Stores settings only for local dev
        - production.py    # Stores settings only used by production (e.g. Heroku)
    - urls.py              # Global urls.py, in turn includes urls.py in apps
    - static/              # Static files
- apps/                    # A directory to store all our custom apps
    - accounts/            # An example custom app that includes sign-up and log-in
        - models.py        # Customized 
        - urls.py          # URLs for sign-up and log-in pages
        - views.p          # Views for sign-up and log-in pages
    - homepage/            # An example custom app that has some static pages
        - etc
```



## Launching to Heroku

* Prereq: [You have Heroku and Postgres installed and set-up.
  ](https://github.com/kickstartcoding/postgres-getting-started)





<!-- {% endif %} -->

# {{ project_name }} - Django project

A Django project built using [Kickstart Coding's Django Project Starter](http://kickstartcoding.com/)

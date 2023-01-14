# Welcome to Wagtail ecommerce Documentation

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

``` mermaid
graph TD
    A[Christmas] -->|Get money| B(Go shopping)
    B --> C{Let me think}
    C -->|One| D[Laptop]
    C -->|Two| E[iPhone]
    C -->|Three| F[fa:fa-car Car]
```

## Quick install
Run the following commands in a virtual environment of your choice:

    pip install wagtail

(Installing wagtail outside a virtual environment may require sudo. sudo is a program to run other programs with the security privileges of another user, by default the superuser)

Once installed, Wagtail provides a command similar to Django’s django-admin startproject to generate a new site/project:

    wagtail start mysite

This will create a new folder mysite, based on a template containing everything you need to get started. More information on that template is available in the project template reference.

Inside your mysite folder, run the setup steps necessary for any Django project:

    pip install -r requirements.txt
    python manage.py migrate
    python manage.py createsuperuser
    python manage.py runserver

Your site is now accessible at http://localhost:8000, with the admin backend available at http://localhost:8000/admin/.

This will set you up with a new stand-alone Wagtail project. If you’d like to add Wagtail to an existing Django project instead, see Integrating Wagtail into a Django project.
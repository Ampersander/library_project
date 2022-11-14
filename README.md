# Django Library

## Overview

The main features that have currently been implemented are:

* There are models for libraries, books, book copies, genre, language and authors.
* Users can view list and detail information for books and authors.
* Admin users can create and manage models. The admin has been optimised 
* Librarians can renew reserved books
* Authentication, for two types of profiles: bookseller and customer
* Reading groups, with session planning (doodle like)
* Search for book and library proposing it
* Selection of libraries by geographical area
* Chat/forum
* Back office for libraries:
`* added books`
`* loan management interface`
`* list of book return delays`
`* creation of reading groups`
* client homepage:
`* reminder of the next groups of readings`
`* reminder of books to return`

## Quick Start

To get this project up and running locally on your computer:
1. Set up the [Python development environment](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/development_environment).
   We recommend using a Python virtual environment.
   > **Note:** This has been tested against Django 3.1.2 (and may not work or be "optimal" for other versions).
1. Assuming you have Python setup, run the following commands (if you're on Windows you may use `py` or `py -3` instead of `python` to start Python):
   ```
   pip3 install -r requirements.txt
   python3 manage.py makemigrations
   python3 manage.py migrate
   python3 manage.py collectstatic
   python3 manage.py test # Run the standard tests. These should all pass.
   python3 manage.py createsuperuser # Create a superuser
   python3 manage.py runserver
   ```
1. Open a browser to `http://127.0.0.1:8000/admin/` to open the admin site
1. Create a few test objects of each type.
1. Open tab to `http://127.0.0.1:8000` to see the main site, with your new objects.

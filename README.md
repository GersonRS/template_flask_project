# Template flask project
This script will start a new Flask project on the application factory model.      

## Structure provided
~~~sh
<project name>/
+-- <project name>/
|   +-- ext/ 
|   |   +-- site/
|   |   |   +-- __init__.py
|   |   |   +-- main.py
|   |   +-- __init__.py
|   +-- static/
|   |   +-- ccs/
|   |   +-- img/
|   |   +-- js/
|   +-- templates/
|   +-- __init__.py
|   +-- app.py --> project entry point
+-- tests/
|   +-- conftest.py
|   +-- test_app.py --> with 3 tests
+-- LICENCE
+-- Makefile
+-- README.md
+-- requirements.txt
+-- requirements-dev.txt
+-- setup.py
~~~

## How to use
2. Run with the command:
~~~sh
$ python3 startproject.py your_project_name --venv
~~~
> IMPORTANT
> - Do not use spaces in your project name.  Prefer underscores instead spaces.
> - The `--venv` argument indicates that you want to create a virtual environment.  It will be created inside the project's root folder as `.venv`.   

In the `Makefile` file, we have some useful commands, which we use with the `make` command, such as:   

| **command**        | **what he does**                                  |
|--------------------|---------------------------------------------------|
| `make clean`       | clears the project folder                         |
| `make install`     | install our project as a package python           |
| `make install-dev` | similar to install, but with requirements-dev.txt |
| `make test`        | run tests                                         |
| `make run`         | run flask                                         |
| `make run-dev`     | run flask in the development environment          |

---

This python script was created by Gerson during [NExT](https://www.cesar.school/next-nova-experiencia-de-trabalho/) taught by Gerson.

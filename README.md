# Template flask project
This script will start a new Flask project on the application factory model.      

## Structure provided
~~~sh
.
├── <project name>
│   ├── app.py --> project entry point
│   ├── ext
│   │   ├── admin.py
│   │   ├── api
│   │   ├── auth
│   │   ├── cli.py
│   │   ├── config.py
│   │   ├── db
│   │   │   ├── commands.py
│   │   │   ├── __init__.py
│   │   │   └── models.py
│   │   ├── __init__.py
│   │   ├── site
│   │   │   ├── __init__.py
│   │   │   └── main.py
│   │   └── toolbar.py
│   ├── __init__.py
│   ├── static
│   │   ├── css
│   │   ├── img
│   │   └── js
│   └── templates
│       └── base.html
├── LICENCE
├── Makefile
├── README.md
├── requirements-dev.txt
├── requirements.txt
├── secrets.toml
├── settings.toml
├── setup.py
└── tests
    ├── conftest.py
    └── test_app.py --> with 3 tests
~~~

13 directories, 28 files

## How to use
1. Run with the command:
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

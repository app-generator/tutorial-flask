# [Flask](https://palletsprojects.com/p/flask/) Tutorial

> Content provided by experienced developers based on the suggestions/questions from the audience. This initiative aims to provide **Free/Allways up-to-date** programming tutorials - Read the [Manifest](https://github.com/app-generator/learn-to-code).

<br />

## How it works

- Access the existing content
- Open a [new issue](https://github.com/app-generator/tutorial-flask/issues/new) to get an answer related to an existing topic
- Open a [new issue](https://github.com/app-generator/tutorial-flask/issues/new) to open a new tutorial topic
- Answers will be provided by experienced contributors 
- For [Support](https://appseed.us/support/) chat with `AppSeed` team 

<br /> 

## Topics 

- [What is Flask](#what-is-flask)
- [Install Flask](#install-flask)
- [A minimal Flask application](#a-minimal-app)
- [Flask Project Structure](#flask-project-structure) - a few options
- (WIP) [Flask Bootstrap Sample](#flask-bootstrap-sample) - a simple project built with Bootstrap
- (WIP) [Jinja Template](#jinja-template) - how to render HTML pages efficiently

<br />

## What is Flask

:point_right: Flask is a lightweight web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications.
Compared to [Django](https://www.djangoproject.com/), Flask provides a lightweight codebase and more freedom to the developer.

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## Install Flask

:point_right: The easiest way to install [Flask](https://palletsprojects.com/p/flask/) is to use [PIP](https://pip.pypa.io/en/stable/quickstart/) the official package-management tool.

```bash
$ pip install Flask
```

<br />

**How to check Flask version**

Open a Python console (type python in terminal) and check the installed version as below:

```python
>> import flask
>> flask.__version__
'1.1.2' 
>>>
```

In this case the installed version is **1.1.2**

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## A minimal App

:point_right: Open a terminal and install Flask (if not already installed) using PIP:

```bash
$ pip install Flask
```

Use your preferred editor to create a file called **hello.py** with this content:

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def hello():
    return f'My first Flask!'
```

Save the file and start the app:

<br />

```bash
$ env FLASK_APP=hello.py flask run
 * Serving Flask app "hello"
 * Running on http://127.0.0.1:5000/
```

Above commnand does two things:

- Set the `FLASK_APP` variable (required by Flask)
- Execute our code with `flask run` command

<br />

By visiting the app in the browser **localhost:5000** we should see **My first Flask!** message.

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## [Flask Project Structure](./flask-project-structure.md)

:point_right: Being such a lightweight framework, Flask comes with great flexibility regarding the codebase structure of a project. We can use a single file and drop all the code or split the app logic in more files and directories. All variants works but we migth have issues once our project is getting bigger and migth become unreadable for others. 

Well, this section presents a few options to keep in mind when we start a Flask project. 

<br />

> :link: Read more: [Flask Project Structure](./flask-project-structure.md): [Single File](./flask-project-structure.md#single-file), [Isolated App](./flask-project-structure.md#isolated-app-directory), [Blueprints](./flask-project-structure.md#blueprints)

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## [Flask Bootstrap Sample](./flask-bootstrap-sample.md)

:point_right: We can use the information learned in the previous sections and build from scratch a simple Flask project on top of a modern Bootstrap UI Kit.

<br />

> :link: Read more: [Flask Bootstrap Sample](./flask-bootstrap-sample.md)

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## [Jinja Template](./jinja-template.md)

:point_right: Jinja is a modern and designer-friendly templating language for Python, modelled after Django's templates. It is a text-based template language and thus can be used to generate any markup as well as source code.

<br />

> :link: Read more: [Jinja Template](./jinja-template.md)

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

---
**[Flask](https://palletsprojects.com/p/flask/) Tutorial** - Free/Allways up-to-date Flask-related content | by [AppSeed](https://appseed.us?ref=gh).

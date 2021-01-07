# Flask Bootstrap Sample

> Part of [Flask Tutorial](https://github.com/app-generator/tutorial-flask): Learn how to built from scratch a simple Flask project by using an open-source Bootstrap UI Kit.

**Spot an issues or want to contribute?** - use the [Issues Tracker](https://github.com/app-generator/tutorial-flask/issues/) and tell us more. 

<br />

## Topics

- [What is Bootstrap](#what-is-bootstrap)
- [Swipe - Bootstrap UI Kit](#swipe-bootstrap-ui-kit)
- [Project Structure](#project-structure)
- [Assets Management](#assets-management)
- [Jinja Templates](#jinja-templates)
- [Create New Pages](#create-new-pages)
- [Summary](#summary)

<br />

## What is Bootstrap

:point_right: Bootstrap is a free and open-source framework that contains CSS and JavaScript-based design templates for typography, forms, buttons, navigation, and other interface components. Using Bootstrap in our work, we might code faster the UI by reusing the elements provided in this popular library. 

- [Bootstrap](https://getbootstrap.com/) - the official website
- [Bootstrap Docs](https://getbootstrap.com/docs/5.0/getting-started/introduction/) - explain in deep how to get started

In our sample we will use more than just Bootstrap: Swipe is a modern, open-source UI Kit released under MIT License on Github. The permissive license allows unlimited copies for hobby and commercial projects.  

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## Swipe Bootstrap UI Kit

:point_right: This open-source UI Kit can be downloaded directly from the public repository: [Swipe - One Page Bootstrap 5](https://github.com/themesberg/swipe-one-page-bootstrap-5). The project comes with three pages:

- Landing page
- Sign In (login)
- Sign Up (register)

This design will be integrated in our Flask project.  

<br />

![Swipe - Open-Source Bootstrap 5 UI Kit.](https://raw.githubusercontent.com/app-generator/tutorial-flask/main/media/swipe-bootstrap-5.png)

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## Project Structure

:point_right:  Flask comes with great flexibility regarding the codebase structure of a project. The sample presented in this page will use a clean and intuitive file-structure presented in detail in **[Flask Project Structure](./flask-project-structure.md)** chapter on this tutorial as **[Isolated app directory](./flask-project-structure.md#isolated-app-directory)** pattern. 

<br />

**The project structure**

```bash
< PROJECT ROOT >
   |
   |-- app/
   |    |
   |    | -- views.py                      # App Routing
   |    | -- __init__.py                   # Expose the Flask Application object 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |
   |    |-- templates/
   |    |    |
   |    |    |-- includes/                 # Page chunks, components
   |    |    |    |
   |    |    |    |-- navigation.html      # Top bar
   |    |    |    |-- scripts.html         # JS scripts common to all pages
   |    |    |    |-- footer.html          # The footer component
   |    |    |
   |    |    |-- layouts/                  # App Layouts (the master pages)
   |    |    |    |
   |    |    |    |-- base.html            # Used by index page
   |    |    |    |-- base-fullscreen.html # Used by auth pages 
   |    |    |
   |    |    |-- accounts/                 # Auth Pages (login, register)
   |    |    |    |
   |    |    |    |-- login.html           # Use layout `base-fullscreen.html`
   |    |    |    |-- register.html        # Use layout `base-fullscreen.html`  
   |    |    |
   |    |  index.html                      # The default page
   |
   |-- requirements.txt                    # Application Dependencies
   |
   |-- run.py                              # Start the app in development and production
   |
   |-- *************************************
```

<br />

> Relevant Files and folders

- `run.py` - is the entry point called to start the app
- `app/__init__.py` - constructs the application
- `views.py` - define app routing
- Static assets and template folders:
    - `static`: the place where JS,Images and CSS files are saved
    - `templates`: pages and components to be used 

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## Assets Management

:point_right: Assets are copied from the HTML version preserving the structure: 

```bash
```bash
< PROJECT ROOT >
   |
   |-- app/
   |    |
   |    |-- static/
   |         |-- css      # CSS files
   |         |-- img      # Images 
   |         |-- js       # Javascript Files
   |     
   |
   |-- *************************************   
```

By default `Flask` will serve the assets from  a directory with name `static` located in the current folder. This can be changed with ease when `Flask` constructor is invoked:

```python

app = Flask(__name__,
            static_url_path='', 
            static_folder='web/static')
```

In this code snippet Flask constructs the application loading the assets from a subfolder `web/static`.   

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## [Jinja Templates](./jinja-template.md)

:point_right: ToDo

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## Create New Pages

:point_right: ToDo

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

## Summary

:point_right: ToDo

<br />

<p align="right"><a href="#topics"> :point_up_2: Return to top</a></p>

<br />

---
**Flask Bootstrap Sample** - [Flask Tutorial](https://github.com/app-generator/tutorial-flask) | by [AppSeed](https://appseed.us?ref=gh).

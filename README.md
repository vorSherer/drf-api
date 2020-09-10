# Lab 31 - Django REST Framework and Docker

### *Author: Thomas Sherer*, 2020-09-10

---

## Description
### Overview
Use Django REST Framework to create an API, then "containerize" it with Docker.

## Feature Tasks and Requirements
- Rebuild from scratch a custom version of __`Blog API`__ demo project that is not a blog project.
	- Replace __`Blog`__ and __`Post`__ with your own application and model.
	- Your model must have at least as many fields as demo’s model.
	- Your model must have one field that is a foreign key to user.
	- *__NOTE__: You are not required to build any templates for this lab.* <br>

## Features - Docker
- *__NOTE__: Refer to the class demo for built out __`Dockerfile`__ and __`docker-compose.yml`__ examples.*
- Update __`Dockerfile`__ and __`docker-compose.yml`__ if needed. <br>

## Implementation Notes
- You'll need to run a command to convert pyproject.toml dependencies to requirements.txt <br>
	- poetry export -f requirements.txt -o requirements.txt

- If you get an __`allowed host`__ error examine the bug details and update code as needed.
- When __Docker__ is installed and docker files are ready to go then run… <br>
	- $ __*docker-compose up*__
- To shut docker down enter __`ctrl+c`__
- You’ll learn a better way soon

## User Acceptance Tests
Modify provided unit tests in demo to work for your project.

## Configuration
Use __`poetry`__ to initialize __`drf-api`__ project.

    - $ mkdir drf-api

    - $ cd drf-api

    - $ poetry init -n

    - $ poetry shell

Then continue to build the Django project.

Use the __`drf-api`__ folder as the root of your project’s git repository.
 <br>

---

## Collaborations and Attributions
<!-- __Skyler Burger__ helped with NN. -->

<!-- __Merry Cimakasky__ helped with NN. -->

<!-- __Lee-Roy King__ helped with NN. -->

.gitignore content courtesy of https://www.toptal.com/developers/gitignore/api/django

<!-- __likegeeks.com__ helped with [understanding chr() and ord()](https://likegeeks.com/python-caesar-cipher/) -->

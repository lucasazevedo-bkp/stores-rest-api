# Stores REST API
> Stores, Items and Authentication REST API with Flask (Restful & JWT & SQLAlchemy).
>
> [Course](https://www.udemy.com/course/rest-api-flask-and-python/) | [Certificate](https://ude.my/UC-bd2aaca2-7b89-4c77-beeb-7ad63e292107)

![Ubuntu Version](https://img.shields.io/badge/ubuntu-20.04-blue)
![Python Version](https://img.shields.io/badge/python-3.8.10-blue)
![SQLite Version](https://img.shields.io/badge/sqlite-3.x-blue)
![Flask Version](https://img.shields.io/badge/flask-2.0.2-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## Installation

Create and activate a virtual environment in the root directory:

```sh  
python -m venv .venv
source .venv/bin/activate
```

Install the requirements:

```sh  
pip install -r requirements.txt
```

Add an .env file with the following variables:

```sh  
# .env content
# for example, FLASK_ENV=development
FLASK_ENV=
FLASK_SECRET_KEY=
```

Run Flask:

```sh  
flask run
```

Endpoints:

```sh
POST http://localhost:5000/register {"username": "<username>", "password": "<password>"}
POST http://localhost:5000/auth {"username": "<username>", "password": "<password>"}
GET http://localhost:5000/items
GET http://localhost:5000/item/<name> 
POST http://localhost:5000/item/<name> {"price": "<price>", "store_id": "<store_id>"}
PUT http://localhost:5000/item/<name> {"price": "<price>", "store_id": "<store_id>"}
DEL http://localhost:5000/item/<name> 
GET http://localhost:5000/stores
GET http://localhost:5000/store/<name>
POST http://localhost:5000/store/<name>
DEL http://localhost:5000/store/<name>
```
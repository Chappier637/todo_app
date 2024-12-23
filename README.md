# todo-app

## Descriprion

This is a learning prokect for Data Engineering program at HSE.

The goal is to create TODO-app-like service using FastAPI

## Methods

- GET /items - returns full list of ToDo items
- GET /items/{item_id} - returns iten of given item_id
- POST /items - adds given ToDo item into list
- PUT /items/{item_id} - updates existing item_id item
- DELETE /items/{item_id} - deletes existing item_id item

## Deployment

### Github

- Clone github project
```
  git clone https://github.com/Chappier637/todo_app.git
```
- Switch to app directory
```
  cd app
```
- Update pip and install modules from requirements.txt
```
  python3 -m pip install --upgrade pip
```
```
  pip install -r requirements.txt
```
- Compiling docker image
```
  docker build -t <your path> .
```
- Start docker container
```
  docker run -d -p 8000:80 -v todo-data:/app/data <your image name>
```

### From Docker
```
docker run -d -p 8000:80 -v shortner-data:/app/data tymerrit/todo-sqlite
```

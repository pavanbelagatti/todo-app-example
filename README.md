# Todo list exercise

## Prerequisites 

- [nodejs](https://nodejs.org/en/)
> - [docker](https://docs.docker.com/) and [docker-compose](https://docs.docker.com/compose/)
> - [helm](https://helm.sh/) and [minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/)

## Install

```sh
git clone https://github.com/thobalose/todo-list-app.git ; cd todo-list-app/
```

```sh
npm install
```

## Run

```sh
node app.js
```

Visit http://localhost:8080 in your browser

## Test

To run tests

```sh
npm test
```

## Docker

To build a docker image for the todo-list-app and run it inside a container execute

```sh
docker build -t thoba/todo-list-app .
```

The above with create an image with the `latest` tag. To run the container execute

```sh
docker run -it -p 8080:8080 --name todo_list_app thoba/todo-list-app
```

You can also use `docker-compose` if you have it installed. To build and run the latest source using `docker-compose` execute

```sh
docker-compose up --build -d
```

and visit http://localhost:8080 in your browser

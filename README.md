# hello-vue + Django

This is a boilerplate project for using vuejs with Django. Forked from: https://github.com/rokups/hello-vue-django
I'll keep this project up-to-date and add useful instructions that might be helpful :-D

### Features

* Django backend in `./backend`
* vuejs (v2) frontend in `./frontend`
* Hot-reload with vue-loader
* eslint linter integration
* Makefile to make your life easy

### Start Project
Run the following command to start a new project, change projectname to your project's name:
`django-admin startproject projectname --template https://github.com/timtech4u/hello-vue-django/archive/master.zip`


### Development environment setup

These steps will install all required dependencies including development ones, run migrations and start dev server.

```bash
make dev
make migrate
make run
```

### Deployment

These steps will install productio dependencies and build vuejs application to `static/dist` folder.

```bash
make prod
make build
```

### Be aware

For the sake of simplicity Django config is contained within it's own backend app. In real world setting you would
probably want to remove `backend` from `INSTALLED_APPS`, create a new app and move `backend.views` to it.

You probably want to create python virtual environment as well. Default python instance available will be used.

### API and CORS Support
If you'll be building an API endpoint you'll probably need to setup Django Cors...

Full Instructions can be found at: https://github.com/ottoyiu/django-cors-headers

### UI Frameworks
Checkout: https://cssauthor.com/vuejs-frameworks/

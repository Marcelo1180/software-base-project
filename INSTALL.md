# Base Project

## Requirements

- Git
- Vagrant
- Ansible

## First

Cloning repos into root of project
```sh
git clone git@github.com:Marcelo1180/django-base-backend.git 
```

## Second

Setup gitconfig
```sh
cp config.example.yml config.yml
vim config.yml
gitconfig:
  - {name: "user.name",  value: "Your name here" }
  - {name: "user.email", value: "demo@email.com" }
  - {name: "ui.color",   value: "u'True'" }
```

## Third

Start the machine
```sh
vagrant up
```

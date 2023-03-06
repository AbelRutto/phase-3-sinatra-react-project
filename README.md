# Phase 3 Project Guidelines


# Project Task Management API

This project management API is a simple web API where you make CRUD calls to a server to organize a project management app.

[demo here]()

## Front-end Project Task Management Interface

You can use this API in conjunction with my front-end project management app [see the repo](https://github.com/AbelRutto/Task-Manager-App)

## Technologies Used in API

- Ruby
- ActiveRecord
- SQLite3
- Rack

## local host 
`http://localhost:3001`

## How To Use

Install it and run:

```sh
bundle install

# create migrations with activerecord
rake db:migrate

# if you would like to use seed data
rake db:seed

# start server
rake start

## Relationships within Database

### Projects

- has many boards
- has many tasks through boards

### Boards

- belongs to a project
- has many tasks

### Tasks

- belongs to a board
- belongs to project though a board

## Example Calls You Can Make With API

### Projects

You can make all CRUD calls for the projects database.

- CREATE projects
- GET/RETRIEVE all projects
- GET/RETRIEVE individual project
- DELETE a project
- UPDATE a project

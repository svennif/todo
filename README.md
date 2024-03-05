# My Todo App

This is a simple todo app built using PHP and SQLite. It allows you to create, update, and delete todos.

## Project Structure

```
my-todo-app
├── src
│   ├── index.php
│   ├── todo
│   │   ├── TodoController.php
│   │   ├── TodoModel.php
│   │   └── TodoView.php
│   └── db
│       └── Database.php
├── tests
│   └── TodoTest.php
├── vendor
├── composer.json
├── .env
└── README.md
```

## Files

- `src/index.php`: This file is the entry point of the application. It handles the routing and rendering of views for the todo app.

- `src/todo/TodoController.php`: This file exports a class `TodoController` which handles the logic for creating, updating, and deleting todos. It interacts with the `TodoModel` and `TodoView` classes.

- `src/todo/TodoModel.php`: This file exports a class `TodoModel` which handles the database operations for the todos. It uses the `Database` class from the `db` directory to connect to the SQLite database.

- `src/todo/TodoView.php`: This file exports a class `TodoView` which handles the rendering of views for the todos. It uses HTML templates to display the todos.

- `src/db/Database.php`: This file exports a class `Database` which provides a wrapper around the SQLite database. It handles the connection and execution of queries.

- `tests/TodoTest.php`: This file contains unit tests for the `TodoController` and `TodoModel` classes. It uses a testing framework like PHPUnit to run the tests.

- `vendor/`: This directory contains the dependencies installed via Composer. It is not included in the project tree structure.

- `composer.json`: This file is the configuration file for Composer. It lists the dependencies required for the project.

- `.env`: This file contains environment variables for the project, such as the database connection details.

## Setup

1. Clone the repository.

2. Install the dependencies using Composer:
   ```
   composer install
   ```

3. Set up the database connection details in the `.env` file.

4. Run the application:
   ```
   php src/index.php
   ```

## Usage

- Open the application in your web browser.

- Create a new todo by entering the task details and clicking the "Add Todo" button.

- Update a todo by clicking the "Edit" button next to the todo and modifying the task details.

- Delete a todo by clicking the "Delete" button next to the todo.

That's it! You can now start using the todo app to manage your tasks.
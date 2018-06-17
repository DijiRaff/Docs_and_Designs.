### Task Manager Summary:
The following features and endpoints will be implemented in the [task manager api](https://github.com/Gidraff/task_manager_api).

#### Core Features:
> A new user can register

> A registered user can login

> An authenticated user can add tasks

> A user can add notes against each task

> A user can edit tasks and notes

> A user can deleted tasks


##### Resources Mapping:
-----------------------------------------
| EndPoints        | HTTP verbs           | Functionality  |
| ------------- |:-------------:| :----- |
| /users/register      | Post | Creates a new user |
| /users/login    | Post      |   User logs in to the system, which returns a JWT if the login is successful. |
| /tasks | Post      |   Creates a new task. |
|/tasks/{id}| Put| Updates an existing task.|
|/tasks | Get | Gets all tasks.|
|/tasks/{id} | Get |  Gets a single task for a given ID. The value of the ID comes from the route parameter.|
|/tasks/users/{id}| Get | Gets all tasks associated with a user. The value of the user ID comes from the route parameter.|
| /tasks/{id} | Delete | Deletes an existing task for a given ID. The value of the ID comes from the route parameter.|
|/notes | Post | Creates a new note against an existing task.|
| /notes/{id} | Put | Updates an existing task note.|
| /notes | Get | Gets all task notes. |
| /notes/{id} | Get | Gets a single note for a given ID. The value of the ID comes from the route parameter.|
| /notes/tasks/{id} | Get | Gets all task notes for a given task ID. The value of the ID comes from the route parameter.|
| /notes/{id} | Delete | Deletes an existing note for a given ID. The value of the ID comes from the route parameter.|
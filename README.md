# Code Tracker API Documentation

## Base URL

- Base URL: `https://localhost/8000`

## Tasks Endpoints

### GET Tasks

- **Endpoint:** `/tasks`
- **Method:** `GET`
- **Description:** Retrieve a list of tasks.

### POST a Task

- **Endpoint:** `/tasks`
- **Method:** `POST`
- **Description:** Create a new task. The unique id will be provided, there is no need to create it.
- **Request Payload:**
  - JSON object: `{ "task": "New Task", "completed": true or false }`
- **Response:**
  - JSON object: `{ "id": "new_task_id", "task": "New Task", "completed": true }`

### Delete a Task

- **Endpoint:** `/tasks/:id`
- **Method:** `DELETE`
- **Description:** Delete a task based on its ID.
- **Request Parameter:**
  - `:id` - ID of the task to be deleted
- **Response:**
  - JSON object: `{ "message": "Task deleted successfully" }`


# Task Tracker CLI

## Description
Task Tracker CLI is a command-line application that allows you to track and manage tasks. Tasks are stored in a JSON file and can be easily added, updated, deleted, and listed from the terminal.

## Features
- Add new tasks.
- Update the description of an existing task.
- Delete tasks.
- Mark tasks as "in progress" or "done".
- List all tasks or filter by status (todo, in progress, done).

## Installation
1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd task-tracker-cli
   ```
2. Ensure you have **Python 3** installed on your system.
3. No external dependencies are required.

## Usage

Run the script from the terminal using the following format:

### Add a task
```sh
python task_tracker_cli.py add "Buy groceries"
```
Expected output:
```sh
Task added successfully (ID: 1)
```

### Update a task
```sh
python task_tracker_cli.py update 1 "Buy groceries and cook dinner"
```

### Delete a task
```sh
python task_tracker_cli.py delete 1
```

### Mark a task as in progress
```sh
python task_tracker_cli.py mark-in-progress 1
```

### Mark a task as done
```sh
python task_tracker_cli.py mark-done 1
```

### List all tasks
```sh
python task_tracker_cli.py list
```

### List tasks by status
```sh
python task_tracker_cli.py list todo
python task_tracker_cli.py list in-progress
python task_tracker_cli.py list done
```

## JSON Structure
Each task stored in `tasks.json` will have the following format:
```json
[
  {
    "id": 1,
    "description": "Buy groceries",
    "status": "todo",
    "createdAt": "2024-01-31T12:00:00",
    "updatedAt": "2024-01-31T12:00:00"
  }
]
```

## Contribution
Contributions are welcome. You can submit a **Pull Request** or report issues in the **Issues** section.

## License
This project is licensed under the MIT License.


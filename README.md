# TO-DO List Tool

A simple, lightweight command-line To-Do List application written in Python. Tasks are stored in a structured JSON file (`memo.json`) for easy reading and management.

## Features
- Add, view, update, and delete tasks
- Persistent storage using JSON
- Clean command-line interface

## Requirements
- Python 3.x

## How to Run
```bash
python main.py
```

## User Manual

### Starting the Program
1. Open a terminal/command prompt.
2. Navigate to the project folder.
3. Run: `python main.py`
4. You will see the welcome menu.

### Available Options (Commands)
The program uses a numbered menu. Type the number and press Enter.

| Option | Command | Description |
|--------|---------|-------------|
| 1 | Create Task | Add a new task. You will be prompted to enter the task description. |
| 2 | View Tasks | Display all your tasks with their status (Not Done / Done). |
| 3 | Mark Task as Done | View tasks, then enter the task number to mark it as completed. |
| 4 | Delete Task | View tasks, then enter the task number to permanently remove it. |
| 5 | Exit | Close the program. |

### Example Session
```
Welcome to TO-DO List Program
1. Create Task
2. View Tasks
3. Mark Task as Done
4. Delete Task
5. Exit

Choose an option: 1
Enter Task: Buy groceries
Task saved successfully!

Choose an option: 2

Your Tasks:
1. Buy groceries | Not Done

Choose an option: 3
Enter task number to mark as done: 1
Task 1 marked as Done!

Choose an option: 5
Exiting To-Do List. Goodbye!
```

### Tips
- Tasks are automatically saved to `memo.json`.
- Task numbers are shown when you view tasks — use those numbers for options 3 and 4.
- Invalid input will show an error message and return you to the menu.

## Project Structure
- `main.py` - Entry point
- `main_loop.py` - Main application loop
- `func.py` - Core functions
- `memo.json` - Task storage file

## License
MIT

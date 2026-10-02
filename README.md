# Simple To-Do List Application
 
A beginner-friendly command-line task manager built with **pure Python**. Add, view, complete and remove tasks, and your tasks are saved to a file so they are still there the next time you run the program.
 
## Features
 
- View all tasks with their status (Done / Not Done)
- Add a new task
- Mark a task as completed
- Remove a task
- Tasks are saved automatically to `tasks.txt` (file persistence)
- Input validation: typing text instead of a number won't crash the program
## Tech Used
 
- Python 3.6 or newer
- Concepts: lists, dictionaries, file handling, functions, loops, exception handling
- Libraries: none (uses only built-in Python)
## Project Structure
 
```
├── todo_list.py       # Main application
├── instructions.txt   # How to use the app
├── requirements.txt   # Dependencies (none required)
└── README.md          # Project documentation
```
 
## How to Run
 
1. Make sure Python is installed:
```bash
   python --version
```
2. Clone this repository or download it as a ZIP:
```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
```
3. Run the program:
```bash
   python todo_list.py
```
   On Mac/Linux you may need to use `python3 todo_list.py`.
 
## Usage
 
```
Options:
1. Display to-do list
2. Add a task
3. Mark a task as completed
4. Remove a task
5. Quit
Enter your choice:
```
 
## How It Works
 
- Tasks are stored in a Python **list** while the program runs. Each task is a dictionary: `{"task": "Buy milk", "completed": False}`.
- `save_tasks()` writes every task to `tasks.txt` after each change. Each line looks like `0|Buy milk` (`0` = not done, `1` = done).
- `load_tasks()` reads `tasks.txt` when the program starts, so your list is restored.
## Learning Outcomes
 
- Working with Python lists and dictionaries
- Reading from and writing to files
- Handling errors with `try / except`
- Organizing code into reusable functions

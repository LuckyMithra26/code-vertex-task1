# code-vertex-task1
A To-Do List Application is a simple yet effective project that helps users manage their tasks and keep track of their daily activities. This application allows users to add, view, update, and delete tasks in their to-do list. It is developed in Python, and it can be built as a command-line application or using a Graphical User Interface (GUI).

Key Features
Add Tasks: Users can add new tasks to the to-do list.
View Tasks: Users can view the list of pending tasks.
Update Tasks: Users can update the status or details of a task.
Delete Tasks: Users can remove tasks from the list.
Task Completion Status: Mark tasks as complete or pending.

Code Explanation:
Data Storage (JSON):
The tasks are stored in a file called tasks.json. We use the json module to read from and write to this file, ensuring that tasks persist between program runs.

Loading and Saving Tasks:
The load_tasks() function tries to load the tasks from the file. If the file doesn't exist, it initializes an empty task list.
The save_tasks(tasks) function saves the current task list into tasks.json so that tasks are retained.

Viewing Tasks:
The view_tasks() function prints out the current list of tasks, each showing its completion status.

Adding a New Task:
In the add_task() function, the user inputs a new task, which is appended to the task list. Each task is represented as a dictionary with two attributes:

title: The name of the task.
completed: A boolean to indicate if the task is done or not.

Updating Task Status:
The update_task() function allows the user to toggle the task’s completion status (from incomplete to complete or vice versa).

Deleting a Task:
The delete_task() function lets the user delete a task from the list by specifying its number.

Main Loop:
The main() function manages the main flow of the program. It repeatedly prompts the user for input (to view, add, update, or delete tasks), and then executes the corresponding function.

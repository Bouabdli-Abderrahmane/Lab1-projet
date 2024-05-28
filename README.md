# Lab1-projet 
This Bash script provides a simple command-line interface for managing tasks, stored in a JSON file (tasks.json). The script supports creating, listing, updating, deleting, showing, and searching tasks by title. It requires jq, a lightweight command-line JSON processor. At initialization, the script checks if the tasks.json file exists and initializes it as an empty JSON array if it doesn't.

The script includes several functions. The create_task function prompts the user for task details (title, description, location, due date) and creates a new task with a unique identifier, which is then appended to tasks.json. The list_tasks function lists all tasks due today, showing their ID, title, and completion status. The delete_task function prompts the user for a task ID and removes the task with the specified ID from tasks.json. The update_task function prompts the user for a task ID and new task details, updating the specified task in tasks.json. The show_task function prompts the user for a task ID and displays the details of the specified task. The search_task_by_title function prompts the user for a title keyword and searches for tasks whose title matches the keyword (case-insensitive).

To use the script, one of six commands must be provided as an argument: create to create a new task, update to update an existing task, delete to delete a task, show to show details of a specific task, list to list tasks due today, or search to search tasks by title. For example, ./script_name.sh create will start the process of creating a new task, while ./script_name.sh list will list tasks due today. If an invalid command is provided, the script displays the correct usage syntax.

In conclusion, this script offers a simple and efficient way to manage tasks from the command line, leveraging JSON for data storage and jq for data manipulation.

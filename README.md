Task Manager  Bot
This project is a Discord bot designed to help small teams manage tasks efficiently. The bot allows users to add, delete, view, and mark tasks as completed. All task data is stored in an SQLite database.

Features
Add a task: Add a new task with a description.

Delete a task: Delete a task by its ID.

View tasks: List all tasks with their IDs and completion status.

Mark a task as completed: Mark a task as completed by its ID.

Commands
Command	Description
!add_task <description>	Adds a new task with the specified description.
!delete_task <task_id>	Deletes the task with the specified ID.
!show_tasks	Lists all tasks with their IDs and descriptions.
!complete_task <task_id>	Marks the task with the specified ID as completed.
Installation
Prerequisites
Python 3.8 or higher

discord.py library

sqlite3 (included with Python)

Steps
Clone the repository:


git clone https://github.com/your_username/task_manager_bot.git
cd task_manager_bot
Install dependencies:


pip install -r requirements.txt
Set up the database:

The bot will automatically create the necessary database and table when it runs for the first time.

Configure the bot:

Replace 'YOUR_DISCORD_BOT_TOKEN' in bot.py with your actual Discord bot token.

Run the bot:


python bot.py
Testing
To run the tests, use the following command:

python run_tests.py
This will execute all the test cases and display the results in the terminal.

Project Structure

task_manager_bot/
├── bot.py                  # Main bot script
├── database.py             # Database connection and setup
├── tests/                  # Test scripts
│   ├── test_add_task.py
│   ├── test_delete_task.py
│   ├── test_show_tasks.py
│   └── test_complete_task.py
├── requirements.txt        # List of dependencies
├── README.md               # Project documentation
└── run_tests.py            # Script to run all tests
Contributing
Contributions are welcome! Please follow these steps:

Fork the repository.

Create a new branch (git checkout -b feature/YourFeatureName).

Commit your changes (git commit -m 'Add some feature').

Push to the branch (git push origin feature/YourFeatureName).

Open a pull request.

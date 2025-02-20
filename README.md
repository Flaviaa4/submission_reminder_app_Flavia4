# submission_reminder_app_Flavia4

## Description
Submission Reminder App is a simple shell script-based app that will alert students about all upcoming assignment deadlines. It sets up the directories and files required for the application to function correctly.

## Features
.Automatically creates a structured directory for the app.
.Populates necessary files including 'config.env,' 'functions.sh', 
 'reminder.sh', 'submissions.txt,' and 'startup.sh'.
.Requests the user's name and personalizes the main directory.
.It will allow students to check pending submissions.
.Ensures scripts are executable
## Directory Structure 
When you run the 'create_environment.sh' script, the following structure will be as follows:

submission_reminder_{YourName}/
│── app/
│   └── reminder.sh
│── config/
│   └── config.env
│── modules/
│   └── functions.sh
│── assets/
│   └── submissions.txt
│── startup.sh

 ## Installation and Setup
 ## 1. cloning the repository
 ...bash
git clone
https://github.com/{githubusername}/submission_reminder_app.git
cd submission_reminder_app
...

## 2. Running the environment Setup Script 
...bash
creating create_environment.sh
You will be asked to enter your name. The script will then create a directory named `submission_reminder_{YourName}` with all necessary files.
...

## 3. Start the Reminder Application
After the environment is set up, navigate to your directory and run:
```bash
cd submission_reminder_{YourName}
bash startup.sh
```
This will load the environment variables, check submissions, and display assignment details.

## Files Descriptions
## `create_environment.sh`
This script sets up the entire environment, creating directories and files required for the application.

## `startup.sh`
Loads environment variables, checks for missing submissions, and displays assignment details.

## 'reminder.sh'
Will check submission status and alert students about pending assignments.

## 'function.sh'
It contains helper functions that will process submission records.

## 'config.env'
stores configuration variables such as the assignment name and deadline.

## 'submissions. txt'
This Contains sample student submission data in CSV format.

 ## Notes
.Ensure you have execution permissions for scripts:
  ...bash
  chmod +x create_environment.sh startup.sh app/reminder.sh modules/functions.sh
  
.Modify `submissions.txt` to add new students or change statuses.
.The script is designed to run on Linux-based system.

**Developed by:**
Flavienne BENIHIRWE

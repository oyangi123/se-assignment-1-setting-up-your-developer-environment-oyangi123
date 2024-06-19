[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/vbnbTt5m)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15283890&assignment_repo_type=AssignmentRepo)
# Dev_Setup
Setup Development Environment

#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. Select Your Operating System (OS):
   Choose an operating system that best suits your preferences and project requirements. Download and Install Windows 11. https://www.microsoft.com/software-download/windows11
   I use Linux Ubuntu
   

3. Install a Text Editor or Integrated Development Environment (IDE):
   Select and install a text editor or IDE suitable for your programming languages and workflow. Download and Install Visual Studio Code. https://code.visualstudio.com/Download
Step 1: Update the System
Open the terminal and update your system package list by running the following commands:
sudo apt update
sudo apt upgrade

Step 2: Install Required Dependencies
Install the required dependencies for Visual Studio Code:
sudo apt install software-properties-common apt-transport-https wget

Step 3: Import the Microsoft GPG Key
Import the Microsoft GPG key by running:
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -

Step 4: Enable the VS Code Repository
Add the Visual Studio Code repository to your system sources list:
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

Step 5: Update the Package List Again
Update the package list again to include the new repository:
sudo apt update

Step 6: Install Visual Studio Code
Install Visual Studio Code by running:
sudo apt install code

Step 7: Launch Visual Studio Code
You can now start Visual Studio Code by either typing code in the terminal or searching for Visual Studio Code in your applications menu.
 
N/B- No problem encountered while installing visual studio

4. Set Up Version Control System:
   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit. https://github.com
   Step 1: Install Git
   On Ubuntu:
   Open your terminal.
   Install Git by running:
   sudo apt update
   sudo apt install git

Step 2: Configure Git
Set your username and email:
git config --global user.name "Oyangi123"
git config --global user.email "oyanggeral@gmail.com"

Step 3: Create a GitHub Account
Go to GitHub.
Click on the "Sign up" button.
Follow the instructions to create a new account.

Step 4: Create a New Repository on GitHub
Log in to your GitHub account.
Click on the "+" icon in the top-right corner and select "New repository".
Fill in the repository name, description (optional), and choose the repository visibility (public or private).
Click "Create repository".

Step 5: Initialize a Git Repository Locally
Open your terminal.
Navigate to your project directory or create a new one:
mkdir software-development
cd software-development

Initialize a new Git repository:
git init
echo "# software-development" > README.md
git add .
git commit -m "this is my first commit"
git push

6. Install Necessary Programming Languages and Runtimes:
  Instal Python from http://wwww.python.org programming language required for your project and install their respective compilers, interpreters, or runtimes. Ensure you have the necessary tools to build and execute your code.

My linux Ubuntu version 22.04 package came with python3 already installed therefore there is no need to install it.

8. Install Package Managers:
   If applicable, install package managers like pip (Python).
Step 1: Update Your Package List
It's always a good idea to update your package list before installing new software. Open your terminal and run:
sudo apt update

Step 2: Install Python and pip
If you don't already have Python installed, you can install it along with pip using the following command. This installs pip for Python 3, which is the standard for most modern Python projects:
sudo apt install python3-pip

Step 3: Verify the Installation
After installation, you can verify that pip was installed correctly by checking its version:
pip3 --version
N/B- No error encountered while installing pip. It was successfull.

10. Configure a Database (MySQL):
   Download and install MySQL database. https://dev.mysql.com/downloads/windows/installer/5.7.html

Step 1: Update Package Index
Before installing any new software, it's always a good practice to update the package index:
sudo apt-get update

Step 2: Install MySQL Server
You can install MySQL Server package using the following command:
sudo apt install mysql-server

During the installation, you'll be prompted to set a root password for MySQL. Make sure to choose a strong password and remember it

Step 3: Secure MySQL Installation
MySQL comes with a script that can perform some security-related operations. You can run this script to secure your MySQL installation:
sudo mysql_secure_installation

Follow the on-screen prompts to complete the security setup. It will prompt you to:

Set the root password (if you haven't already done so during installation).
Remove anonymous users. choose "y"
Disable remote root login. choose "y"
Remove the test database.choose "y"
Reload privilege tables. choose "y"
Troubleshooting
I encountered an error while setting the password. My machine was not accepting the password I was creating. I tried to console ChatGPT but i was not getting the correct solution, at the end i decided to use my local machine password and it worked perfectly.
Step 4: Verify MySQL Installation
After completing the installation and securing MySQL, you can verify that the MySQL service is running by executing:
sudo systemctl status mysql

If MySQL is running, you should see output indicating that the service is active and running.

Step 5: Access MySQL Command Line
You can access the MySQL command line by typing:
mysql -u root -p

You will be prompted to enter the MySQL root password you 
set earlier during installation.


12. Set Up Development Environments and Virtualization (Optional):
   Consider using virtualization tools like Docker or virtual machines to isolate project dependencies and ensure consistent environments across different machines.
Using Docker
Step 1: Install Docker
Ubuntu:
sudo apt update
sudo apt install docker.io


14. Explore Extensions and Plugins:
   Explore available extensions, plugins, and add-ons for your chosen text editor or IDE to enhance functionality, such as syntax highlighting, linting, code formatting, and version control integration.
Extensions to use with visual studio
python extension
Prettier - Code Formatter
ESLint-Integrates ESLint JavaScript into VS Code.
GitLens — Git supercharged: Enhances the Git capabilities in VS Code


16. Document Your Setup:
    Create a comprehensive document outlining the steps you've taken to set up your developer environment. Include any configurations, customizations, or troubleshooting steps encountered during the process. 

#Deliverables:
- Document detailing the setup process with step-by-step instructions and screenshots where necessary.
- A GitHub repository containing a sample project initialized with Git and any necessary configuration files (e.g., .gitignore).
- A reflection on the challenges faced during setup and strategies employed to overcome them.

#Submission:
Submit your document and GitHub repository link through the designated platform or email to the instructor by the specified deadline.

#Evaluation Criteria:**
- Completeness and accuracy of setup documentation.
- Effectiveness of version control implementation.
- Appropriateness of tools selected for the project requirements.
- Clarity of reflection on challenges and solutions encountered.
- Adherence to submission guidelines and deadlines.

Note: Feel free to reach out for clarification or assistance with any aspect of the assignment.

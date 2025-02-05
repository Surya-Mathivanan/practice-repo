# Git Pull & Push Roadmap 
## A Step-by-Step Guide 🚀  
### How to Push Your Code  

This guide helps you set up Git, create a repository, and push & pull your code to GitHub.

## 1.Install Git  
**Why?** Git is a version control system that helps you track changes in your code.  It helps maintain a history of your work and makes collaboration easier.  

🔗 [Download Git](https://git-scm.com/downloads) and install it based on your OS. 
###
![Image](https://github.com/user-attachments/assets/f89f80d8-4d8f-425d-bd38-76de880ccf7d)
---

## 2.Verify Git Installation  
**Why?** To check if Git is installed correctly.  
```sh
git --version
```
---

## 3.Configure Git (Set Username and Email)
**Why?** Git tracks changes using your identity, so it's important to configure your user details before committing any changes to the repository.


```sh
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

```
**Purpose:** The git config command sets your username and email address. This information is attached to each commit to associate changes with your identity.
https://github.com/user-attachments/assets/e3905e94-4b8f-4523-b7d2-15312f979e1b


---

## 4.Open VS Code
**Why?** VS Code is a powerful code editor with Git support.

📌 Open Visual Studio Code from your system.

---
## 5.Create a New Folder and Open in VS Code
**Why?** Creating a dedicated folder for your project keeps your files organized, making it easier to manage..

```sh

mkdir my-project  # Create a new folder
cd my-project     # Navigate into the folder
code .            # Open in VS Code
```
**Purpose:** The mkdir command creates a new directory, cd changes the directory to the newly created folder, and code . opens the folder in VS Code.
---
## 6.Create a New GitHub Repository
**Why?** A GitHub repository stores your project files and version history in the cloud, enabling easy collaboration.

Action: Go to GitHub and create a new repository by clicking "New Repository." Name it, and click "Create Repository."

📌 Steps:
Go to GitHub and log in.
Click New Repository, enter a name, and click Create Repository.
(Optional) Create a file example.txt inside the repository.
---
## 7.Clone the GitHub Repository
**Why?** Copies the repository to your local machine.

```sh

git clone <repository-url>
Replace <repository-url> with your GitHub repo link.
```
https://github.com/user-attachments/assets/c3c552a6-bbb6-4fdf-b708-634e51a0f1ed
---
## 8.Navigate to the Cloned Folder
**Why?** Ensures you're working in the correct project directory.

```sh

cd my-project

```
**Purpose:** The cd command allows you to navigate into the project folder so that you can work on the files.
---
## 9.Create a New File Locally
**Why?** Adds a new file to track with Git.

```sh

touch sample2.txt  # Creates a new file

```
---
## 10.Check Git Status
**Why?** The git status command shows the status of files in your working directory, such as new files or files that have been modified.

```sh

git status
```
**Purpose:** This command checks the current state of the files in your repository, displaying which files have been added, modified, or deleted.
---
## 11.Add the File to Git
**Why?** Before committing changes, files must be staged. Staging adds files to the Git "staging area" in preparation for committing.

```sh

git add sample2.txt
```
**Purpose:** The git add command stages the sample2.txt file, preparing it for commit. Without this step, the changes won't be recorded in the commit.
---
## 12.Commit the Changes
**Why?** Committing is the process of saving the staged changes in your local Git repository with a message describing the update.

```sh

git commit -m "Added sample2.txt"
```
**Purpose:** The git commit command saves your changes in the Git history with a message (-m "message") explaining the changes. This allows you to track your modifications over time.
---
## 13.Push the File to GitHub
**Why?** Pushing your local commits to GitHub uploads your changes to the remote repository, making them available to others.b.

```sh
git push origin main
```
**Purpose:** The git push command uploads your local commits to the GitHub repository. The origin refers to the default name of the remote repository, and main is the branch you're pushing to.
---
## 14.Verify Changes on GitHub
**Why?** After pushing your changes, it's important to verify that they have been successfully uploaded to GitHub.

Action: Go to your GitHub repository and refresh the page to check if the file sample2.txt is visible.



### 📌 Go to your GitHub repository and refresh the page to see sample2.txt.

https://github.com/user-attachments/assets/025f68cd-2b66-47a1-bf85-da30f22fd11e

---


## 15.Setting Up a New Repository
Create a new repository on GitHub.
In your local system, initialize Git:
```
git init
```
```
git remote add origin <repo_url>
```

---
# 16.Deleting a File and Updating GitHub
Delete the file locally.
Stage the deletion:

```
git add .
git commit -m "Deleted unwanted file"
git push origin main
```
The file will also be removed from GitHub.
---

## 17.Pulling Changes from GitHub
**Why?** If there are updates on GitHub that you don’t have locally, git pull fetches the latest changes and merges them into your local repository.

```
git pull origin main
```
**Purpose:** The git pull command fetches updates from the main branch of your GitHub repository and merges them into your local copy.
This command fetches the latest updates from GitHub and merges them into your local repository.
---

## 18.Pulling Latest Changes from Remote
### Before pushing, always pull the latest changes to avoid conflicts:
```
git pull origin main --rebase
```
**Purpose:** The --rebase option fetches the changes and applies your local changes on top of them, preventing merge commits.


### If there are merge conflicts, resolve them manually and continue:
```
git add .
git rebase --continue
```
---
## 19.Handling Errors During Push
**Why?** Errors occur if you try to push changes that conflict with the remote repository. This happens when someone else has pushed updates since your last pull.
If you get an error like:
```
error: failed to push some refs to 'https://github.com/your-username/repository-name.git'
hint: Updates were rejected because the remote contains work that you do not have locally.
```
Solution:
```
git pull origin main --rebase  # Pull the latest changes
git push origin main  # Push again after pulling
```
**Purpose:** The git pull --rebase command gets the latest changes, and git push uploads your local changes after resolving any conflicts.

# Summary of Git Commands:
![Image](https://github.com/user-attachments/assets/e95d5a7d-1be3-4561-9181-636ff75b85ee)







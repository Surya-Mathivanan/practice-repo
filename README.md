# Git Basics: A Step-by-Step Guide 🚀

This guide helps you set up Git, create a repository, and push your code to GitHub.

## 1️⃣ Install Git  
**Why?** Git is a version control system that helps you track changes in your code.  

🔗 [Download Git](https://git-scm.com/downloads) and install it based on your OS.  

## 2️⃣ Verify Git Installation  
**Why?** To check if Git is installed correctly.  
```sh
git --version
```

## 3️⃣ Configure Git (Set Username and Email)
Why? Git tracks changes using your identity.


```sh
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

## 4️⃣ Open VS Code
Why? VS Code is a powerful code editor with Git support.

📌 Open Visual Studio Code from your system.


## 5️⃣ Create a New Folder and Open in VS Code
Why? Organizes project files before using Git.

```sh

mkdir my-project  # Create a new folder
cd my-project     # Navigate into the folder
code .            # Open in VS Code
```

## 6️⃣ Create a New GitHub Repository
Why? A GitHub repository stores your project files and version history.

📌 Steps:
Go to GitHub and log in.
Click New Repository, enter a name, and click Create Repository.
(Optional) Create a file example.txt inside the repository.

## 7️⃣ Clone the GitHub Repository
Why? Copies the repository to your local machine.

```sh

git clone <repository-url>
Replace <repository-url> with your GitHub repo link.
```

## 8️⃣ Navigate to the Cloned Folder
Why? Ensures you're working in the correct project directory.

```sh

cd my-project

```
## 9️⃣ Create a New File Locally
Why? Adds a new file to track with Git.

```sh

touch sample2.txt  # Creates a new file

```
## 🔟 Check Git Status
Why? Shows new or modified files before committing.

```sh

git status
```
## 1️⃣1️⃣ Add the File to Git
Why? Stages the file for the next commit.

```sh

git add sample2.txt
```
## 1️⃣2️⃣ Commit the Changes
Why? Saves the changes in the local Git repository.

```sh

git commit -m "Added sample2.txt"
```
## 1️⃣3️⃣ Push the File to GitHub
Why? Uploads local changes to GitHub.

```sh
git push origin main
```
## 1️⃣4️⃣ Verify Changes on GitHub
Why? Ensures the file is uploaded successfully.

📌 Go to your GitHub repository and refresh the page to see sample2.txt.





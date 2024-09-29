## What is Git and Why is it Powerful?
- Git as a Distributed VCS (Version Control System): Git is a distributed version control system, meaning every developer has a full copy of the repository, enabling decentralized collaboration without needing constant access to a central server.

- Flexibility in Project Sizes: You can use Git for projects ranging from small, single-developer efforts to massive projects with thousands of contributors.

## Checking Git Installation
Git Installation Availability: Git is available for all major operating systems, such as Windows, macOS, and Linux.

Verifying Git Installation: To check if Git is installed on your machine, open a terminal (or command prompt on Windows) and run:

css
```
git --version
```
- This will display the currently installed version of Git if it is present on your computer.

- Installing Git (Windows Example)
## Steps to Install Git on Windows:
- Visit the official Git website for Windows.
- Download the installer (ensure you keep the license agreement as default).
- During installation, choose to install Git with the command line interface.
- Select OpenSSL for security, and enable MinTTY as the terminal emulator.
- You can also enable options 1 and 2 as suggested.


![Screenshot 2024-08-22 100744](https://www.c-sharpcorner.com/article/git-and-github-version-control-local-and-remote-repository/Images/Git%20And%20Github%20Version%20Control.png)

## Git Directory and Working Tree
** Working Tree ** : The working tree is the space where developers work on files. It contains all files currently being tracked by Git. Think of it as a workbench where modifications to files happen.

** Git Directory **: The Git directory acts as the storage for a project’s history. It stores the database of changes and is responsible for tracking all versions of the project. It can be thought of as the repository’s core, keeping track of all file snapshots.

## Staging Area (Index)
- The staging area (also called the index) is an intermediate area where Git stores updates before committing them. Files placed in this area are ready for inclusion in the next commit.
## Git Commands:
** git status ** : This command provides details about the working tree, such as pending changes and the current state of tracked and untracked files.

**git commit** : Used to save changes in the repository. A commit message is required, and Git will abort the process if an empty message is provided. Commit messages should be concise yet informative, containing a short description (ideally under 50 characters), followed by optional additional details within 72-character lines.

![Screenshot 2024-08-22 100744](https://devmountain.com/wp-content/uploads/2022/01/Gitvs_Github-1a-1.jpg)


## File States in Git
- Git projects have three main components:

- **Git Directory**: Contains all the history of tracked files.
- **Working Tree** : Represents the current state of the project, including all files that have been changed but not yet committed.
- **Staging Area** : Holds the changes that are ready to be included in the next commit.
### Tracked and Untracked Files
## Tracked Files : Files that Git is monitoring. These files can be in one of the three states:
- **Modified** : The file has been changed but not yet staged.
- **Staged** : The file has been marked for the next commit.
- **Committed** : The file has been saved into the repository’s history.
## Untracked Files:
- Files that are not being tracked by Git. These files have not been added to the project’s repository yet.

## Modifying, Staging, and Committing Files
- **Modifying Files** : When you modify a tracked file, it enters the "modified" state.
- **Staging Changes** : After modifying a file, it needs to be staged. This step prepares the changes to be included in the next commit.
- **Committing Changes**: Once files are staged, you can commit them to save a snapshot of your project, including all changes made since the last commit.

## Interactive IDE Integration with Git
- Some Integrated Development Environments (IDEs) come with built-in Git interfaces, making it easier to interact with Git through graphical tools instead of command-line operations.

## Git Status Command
- Purpose: The git status command gives you information about the working tree and pending changes. It helps you keep track of what files are staged, modified, or untracked.
## Writing Commit Messages
- Format of Commit Messages: A commit message should contain a short summary (preferably under 50 characters), followed by a blank line, and then a detailed description (less than 72 characters per line). This ensures clarity and consistency in the project's history.
## Main Sections in a Git Project
- A Git project typically has three primary sections:

- **Git Directory**:Stores all the history of the project, including all versions of files.
- **Working Tree** : Represents the current state of your project, including any changes made since the last commit.
- **Staging Area** : Holds the changes that are ready to be committed to the repository.

![Screenshot 2024-08-22 100744](https://github.com/Akshay107app/Version_Control/blob/main/Git/assets/git%20stagging.png?raw=true)


# Git Commit with Flags
- If you want to make a small change and skip the staging step, you can use specific flags in the git commit command:

-m Flag: Allows you to directly add a commit message in the command itself without opening the default editor.

Example: git commit -m "Your commit message"
-a Flag: Automatically stages all tracked files before the commit, which eliminates the need for git add for modified files.

Example: git commit -a -m "Commit message"
Viewing a Specific Commit
If you want to see the details of a specific commit using the commit ID:

git show <commit-id>: This command shows detailed information about the specific commit, including the patch (changes made).
Using the -P Flag in Git Commands
-P Flag: Stands for "Patch." It allows you to view changes in patch format, showing differences between file versions.
git log with -P: You can use git log -p to display the commit history with corresponding patches (i.e., detailed diffs of changes).
Git Checkout
The git checkout command allows you to:

Switch between different branches or restore files.
Revert changes made to a file back to the state in the previous commit.
Purpose: Restores files to the latest committed version, undoing any changes made to files before they are staged.

Example: git checkout <branch_name> or git checkout <file_name>.
Git Amend
git commit --amend: This allows you to modify or update the most recent commit. It overwrites the previous commit, including the message or changes.
Git Revert
git revert: Creates a new commit that undoes the changes made in a specific commit, without deleting the history. It rolls back the changes but keeps a record of the original commit.
Key Terms:
Patch (-P flag): A formatted difference between two versions of a file. It shows line-by-line changes in the code.

git checkout: A command to switch between branches or restore files to an earlier version based on the last commit.

git commit --amend: A command to overwrite or amend the most recent commit, allowing modification of the commit message or included files.

git revert: A command to create a new commit that undoes changes from a previous commit while keeping the commit history intact.


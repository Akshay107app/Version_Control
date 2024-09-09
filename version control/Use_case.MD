- **Commit** : A command to make edits to multiple files and treat that collection of edits as a single change
- **Commit files** : A stage where the changes made to files are safely stored in a snapshot in the Git directory
- **Commit message** : A summary and description with contextual information on the parts of the code or configuration of the commit change
- **Diff** : A command to find the differences between two files
- **DNS zone file** : A configuration file that specifies the mappings between IP addresses and host names in your network
- **Git** : A free open source version control system available for installation on Unix based platforms, Windows and macOS
- **Git directory** : A database for a Git project that stores the changes and the change history
- **Git log** : A log that displays commit messages 
- **Git staging area** : A file maintained by Git that contains all the information about what files and changes are going to go into the next commit
- **Modified files** : A stage where changes have been made to a file, but the have not been stored or committed 
- **Patch** : A command that can detect that there were changes made to the file and will do its best to apply the changes
- **Repository** : An organization system of files that contain separate software projects 
- **Source Control Management (SCM)**: A tool similar to VCS to store source code
- **Stage files** : A stage where the changes to files are ready to be committed 
- **Tracked** : A file’s changes are recorded
- **Untracked** : A file’s changes are not recorded
- **Version control systems (VCS)** : A tool to safely test code before releasing it, allow multiple people collaborate on the same coding projects together, and stores the history of that code and configuration
- **Branch** : An independent line of development, allowing for concurrent updates to the project.
- **Commit ID** : A unique identifier assigned to each commit for referencing purposes.
- **Fast-forward merge** : A merge that moves the branch pointer forward when there is no conflicting commit history.
- **Head** : The reference to the latest commit on the current branch.
- **Master** : The default branch in Git, usually representing the main, stable version of the project.
- **Merge conflict** : A conflict that occurs when two commits change the same part of a file, requiring manual intervention to resolve.
- **Rollback** : The act of reverting a repository to a previous commit.
- **Three-way merge** : A merge that involves comparing the two heads and their common ancestor to resolve differences.
----

## Git Branching and Merging Commands
## Keep this table handy while you are getting comfortable using Git branches and merging. Now, it’s time to put your newfound knowledge of Git branches and merging to use!

| Command                  | Explanation & Link                   |
| Command                  | Description                              |
| ------------------------ | ---------------------------------------- |
| `git init`               | Initialize a new Git repository          |
| `git add .`              | Add all files to the staging area        |
| `git commit -m "message"`| Commit staged changes with a message     |
| `git push`               | Push the changes to the remote repository|                                                                                                                                             
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git branch`                 | [$ git branch](https://git-scm.com/docs/git-branch) can be used to list, create, or delete branches.                                                                 |
| `git branch <name>`          | [$ git branch <name>](https://git-scm.com/docs/git-branch) can be used to create a new branch in your repository.                                                     |
| `git branch -d <name>`       | [$ git branch -d <name>](https://git-scm.com/docs/git-branch) can be used to delete a branch from your repository.                                                   |
| `git branch -D <name>`       | [$ git branch -D <branch>](https://git-scm.com/docs/git-branch) forces a branch to be deleted.                                                                       |
| `git checkout <branch>`      | [$ git checkout <branch>](https://git-scm.com/docs/git-checkout) switches your current working branch.                                                               |
| `git checkout -b <new-branch>` | [$ git checkout -b <new-branch>](https://git-scm.com/docs/git-checkout) creates a new branch and makes it your current working branch.                               |
| `git merge <branch>`         | [$ git merge <branch>](https://git-scm.com/docs/git-merge) joins changes from one branch into another branch.                                                        |
| `git merge --abort`          | [$ git merge --abort](https://git-scm.com/docs/git-merge) can only be used after merge conflicts. This command will abort the merge and try to go back to the pre-merge state. |
| `git log --graph`            | [$ git log --graph](https://git-scm.com/docs/git-log) prints an ASCII graph of the commit and merge history.                                                         |
| `git log --oneline`          | [$ git log --oneline](https://git-scm.com/docs/git-log) prints each commit on a single line.                                                                         |


Instructions to Push the File to GitHub:
Create a README.md file (if you haven't already):

In your project directory, create a new file called README.md and paste the Markdown table code above.
You can create the file using a text editor or directly via terminal:
```
touch README.md
```
Add the Markdown content into the README.md file.
Use any text editor like nano or vim (or open the file using a GUI editor) and paste the content above:
```
nano README.md
```
Then paste the table content and save the file.

Run the following Git commands to push to GitHub:
# Initialize a Git repository (if not already initialized)
```
git init
```

# Add the README.md file to the staging area
```
git add README.md
```

# Commit your changes with a message
```
git commit -m "Added a Git branching and merging table"
```

# Add the remote GitHub repository (replace <repository-url> with your actual URL)
```
git remote add origin <repository-url>
```

# Push the changes to the GitHub repository
```
git push -u origin master
```







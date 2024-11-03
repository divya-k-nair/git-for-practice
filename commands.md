# Git Commands Guide

## 1. Initialization
- **Initialize a Git Repository:** This command creates a new Git repository in the current directory.
  - Command: `git init`

## 2. Configuration
- **Set Global Username:** This command sets your global username for Git commits.
  - Command: `git config --global user.name "divya"`
- **Set Global User Email:** This command sets your global email address for Git commits.
  - Command: `git config --global user.email "divyakaladharannair@gmail.com"`

## 3. Repository Status
- **Check the Status of the Repository:** This command shows the state of the working directory and staging area.
  - Command: `git status`

## 4. File Operations
- **Add Files to Staging Area:** This command adds a specific file or all files to the staging area for the next commit.
  - Command: `git add <filename>`
  - Command: `git add .`  # Add all files

- **Remove a File from Staging Area:** This command removes a specific file from the staging area.
  - Command: `git rm --cached <filename>`

- **Restore a Deleted or Modified File:** This command restores a deleted or modified file to its last committed state.
  - Command: `git restore <filename>`
  - Command: `git restore --staged <filename>`  # From staging area

- **Delete a File from Repository:** This command deletes a file both locally and from the Git repository.
  - Command: `rm <filename>`  # Delete locally
  - Command: `git rm <filename>`  # Delete and track in Git
  - Command: `git commit -m "Deleted <filename>"`

## 5. Committing Changes
- **Commit Changes:** This command records the changes in the staging area to the repository.
  - Command: `git commit -m "Commit message"`

## 6. Branch Management
- **Create a New Branch:** This command creates a new branch and switches to it.
  - Command: `git checkout -b <branch-name>`

- **Switch Between Branches:** This command switches to the specified branch.
  - Command: `git checkout <branch-name>`

- **List All Branches:** This command lists all branches in the repository.
  - Command: `git branch`

## 7. Viewing History
- **View Commit History:** This command displays the commit history for the repository.
  - Command: `git log`
  - Command: `git log --oneline`  # Condensed view

## 8. Merging Changes
- **Merge Changes from Another Branch:** This command merges changes from a specified branch into the current branch.
  - Command: `git merge <branch-name>`

## 9. Remote Operations
- **Push Changes to Remote Repository:** This command pushes the committed changes to the specified remote branch.
  - Command: `git push origin <branch-name>`

- **Pull Changes from Remote Repository:** This command fetches and merges changes from the specified remote branch.
  - Command: `git pull origin <branch-name>`

- **Add Remote Repository:** This command adds a new remote repository with the specified URL.
  - Command: `git remote add origin <repository-url>`

- **View Remote Repositories:** This command lists all remote repositories configured for the local repository.
  - Command: `git remote -v`

## 10. Command History
- **Check Command History:** This command shows the history of commands executed in the terminal.
  - Command: `history`
    
## 11.  Clone Repositories

- **Clone a remote repository to local system**  
  `git clone https://github.com/divya-k-nair/git-for-devops.git`

## 12. Checking Repository Status
- **Check the status of your working directory and staging area**  
  `git status`

- **List all files, including hidden ones**  
  `ls -a`

- **View remote repositories**  
  `git remote -v`

## 13. Adding and Committing Changes
- **Add files to the staging area**  
  `git add <filename>`  
  `git add .`

- **Commit changes with a message**  
  `git commit -m "Commit message"`

## 14. Managing Remote Repositories
- **View remote URLs**  
  `git remote -v`

- **Change the remote repository URL**  
  `git remote set-url origin <new-repository-url>`

## 15. Pushing and Pulling Changes
- **Push changes to a remote branch**  
  `git push origin <branch-name>`

- **Pull changes from a remote branch**  
  `git pull origin <branch-name>`

## 16. Branch Management
- **Create a new branch and switch to it**  
  `git checkout -b <branch-name>`

- **Switch between branches**  
  `git checkout <branch-name>`

- **List all branches**  
  `git branch`

## 17. Merging Branches
- **Merge changes from another branch**  
  `git merge <branch-name>`

- **View a concise commit history**  
  `git log --oneline`

## 18. Editing Files and Tracking Changes
- **Open and edit files using vim**  
  `vim <filename>`

- **Track and commit file changes**  
  `git add <filename>`  
  `git commit -m "Updated <filename>"`

## 19. Working with SSH
- **Change the remote URL to SSH**  
  `git remote set-url origin git@github.com:divya-k-nair/git-for-devops.git`

## 20. Command History
- **View the list of previously executed commands**  
  `history`

## 21. Example Workflow
1. **Clone repository and navigate to it**  
   `git clone https://github.com/divya-k-nair/git-for-devops.git`  
   `cd git-for-devops`

2. **Add a README file and push changes**  
   `vim README.md`  
   `git add README.md`  
   `git commit -m "README.md added"`  
   `git push origin main`

3. **Create and merge branches**  
   `git checkout -b staging`  
   `git checkout -b dev`  
   `git add branching.md`  
   `git commit -m "added branching.md"`  
   `git checkout staging`  
   `git merge dev`  
   `git push origin staging`

4. **Track additional changes and push updates**  
   `git add newfile.md`  
   `git commit -m "5 branches list


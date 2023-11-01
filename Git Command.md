
 **Initializing a New Project:**
1) git init        //(To initialise a new project with Git)
2) git add .     //(Add all files to version controls) 
3) git status    //(Check the status of your Git repository)
4) git commit -m "Commit 1: Initial project setup"   //(Commit your changes with a message)

 **Setting Up Your Repository on GitHub:**
1) git remote add origin https://github.com/AbdullahAnxari/flutter_2023.git      //(To add origin) 
2) git remote -v   //(To check remote repository)
3) git branch  //(To check the branch name) 
4) git branch -M main   //(Create and assign the 'main' branch)


 **Pushing/Uploading Your Code to GitHub:** (push command)
1) git push -u origin main   //(To upload/push on GitHub at the specified branch. The `-u` flag sets the upstream branch, making future pushes easier.)
2) git push   //(No need to write origin main again because of -u)


 **Git Committing and Pushing Changes:**
1) git add .      //(To track all the files)
2) git status    //(To check the status of the git)
3) git commit -m 'Commit 2: Add new button widget'     //(To commit all the tracking files)
4) git push -u origin main  or git push   //(To push your changes to GitHub's 'main' branch)


**Creating and Switching to a New Branch:**
1) git checkout -b 'branch name'  //(Create a new branch and switch to it)
2) git switch 'branch name'    //(Switch to an existing branch)
3) git branch -d "branch name" //(To delete the branch) (this will not delete the file u are in but other files)


**Merging the code**
1) git diff  main   //(It will show the diff main from feature)
2) git merge main   //(It will merge the changes automatically)
3) git diff feature   // (Displays the differences between the current branch and 'feature'.)
4) git merge feature   // Automatically merges changes from the 'feature' branch into the current branch.


**Fetch**
1) git fetch --all --prune   //(It will fetch all the changes from all the branche)


**Pull Your Code to Local:**
1) git pull origin 'file name'



**Fork the code**


**Undoing changes**
1) git restore --staged 'file name'  //(It will restore the changes that you just made in that files)
2) Also use **VS-CODE Git button** to revert changes


**History**
1) git log //(It will show all the commits)


**Delete**
1)rm -rf 'Files name' //(it will remove the file)


**Undo Delete**
1) git reset 'commit id name' //(It will undo delete and take you back to the commit id you write) 


**Add File**
1) git touch 'File name' //(It will create the file) 


**Git Stash:**
1)  git stash save "Your message"   //(Saves your changes in a new stash with a descriptive message.)
2)  git stash list   //(Lists all stashes with unique references (e.g., stash@{0}).)
3)  git stash apply   //(Applies the latest stash to your working directory.)
4)  git stash apply stash@{n} //(Applies a specific stash by referencing its name (e.g., stash@{2}).)
5)  git stash pop   //(Applies and removes the latest stash.)
6)  git stash pop stash@{n}   //(Applies and removes a specific stash.)
7)  git stash show stash@{n}   //(Shows the changes in a specific stash.)
8)  git stash branch branch_name stash@{n}   //(Creates a new branch from a specific stash.)
9)  git stash clear   //(Removes all stashes.)
10)  git stash drop stash@{n}   //(Removes a specific stash without applying it.)
11)   git stash branch new_branch   //(Creates a new branch from the stash and applies the changes to it.)
12)  git stash branch new_branch stash@{n}   //(Creates a new branch from a specific stash and applies its changes.)


**Clone a Git repository from a remote URL to your local machine**
1) git clone https://github.com/your-username/your-repo.git


**Navigate to an Inner Folder**  
1) cd inner-folder // Change Directory to the Inner Folder used after cloning.


**General Commands**
1) ls           // List files and directories in the current folder.
2) ls -a       // List of all files including hidden files.
3) cd         // Change the current directory.
4) cd. .       // To back to main directory
5) pwd      // Print the current working directory.
6) mkdir    // Create a new directory.
7) rm         // Remove files or directories (use with caution)

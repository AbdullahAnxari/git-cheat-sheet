
 **Initializing a New Project:**
1) git init        //(To initialise a new project with Git)
2) git add .     //(Add all files to version controls) 
3) git status    //(Check the status of your Git repository)
4) git commit -m "Commit 1: Initial project setup"   //(Commit your changes with a message)

 **Setting Up Your Repository on GitHub:**
	1) git remote add origin https://github.com/AbdullahAnxari/flutter_2023.git      //(To add origin) 
1) git remote -v   //(To check remote repository)
2) git branch  //(To check the branch name) 
3) git branch -M main   //(Create and assign the 'main' branch)


 **Uploading/Pushing Your Code to GitHub:** (push command)
1) git push -u origin main   //(To upload/push on GitHub at the specified branch. The `-u` flag sets the upstream branch, making future pushes easier.)
2) git push   //(No need to write origin main again because of -u)

**Pull Your Code to Local:**
1) git pull origin 'file name'


 **Git Committing and Pushing Changes:**
1) git add .      //(To track all the files)
2) git status    //(To check the status of the git)
3) git commit -m 'Commit 2: Add new button widget'     //(To commit all the tracking files)
4) git push -u origin main    //(To push your changes to GitHub's 'main' branch)


**Creating and Switching to a New Branch:**
1) git checkout -b 'branch name'  //(Create a new branch and switch to it)
2) git switch 'branch name'    //(Switch to an existing branch)
3) git branch -d "branch name" //(To delete the branch) (this will not delete the file u are in but other files)


**Merging the code**
1) git diff  main  //(It will show the diff main from feature)
2) git merge main  //(It will merge the changes automatically)


**Fork the code**


**Undoing changes**
1) Stage Changes for a Commit


**Clone a Git repository from a remote URL to your local machine**
1) git clone https://github.com/your-username/your-repo.git
2) i.e. git clone https://github.com/AbdullahAnxari/flutter_2023.git 


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





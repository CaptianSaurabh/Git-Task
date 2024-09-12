Based on what you have learnt in the class, do the following steps: 
a. Create a new folder 
b. Put the following files in the folder
                          Code.txt 
                          Log.txt 
                          Output.txt 
c. Stage the Code.txt and Output.txt files 
d. Commit them 
e. And finally push them to GitHub

## 1.Step a: Create a new folder
To create a new folder, you can use the command line interface (CLI) or your operating system's file explorer. Let's assume you're using the CLI. Open your terminal and type the following command
# Command..
mkdir myfolder

## 2.Step b: Put the following files in the folder
Create the following files inside the myfolder directory:
# Command..
cd myfolder
touch Code.txt Log.txt Output.txt

## 3.Step c: Stage the Code.txt and Output.txt files
To stage the Code.txt and Output.txt files, use the following Git commands:
# Command..
git add Code.txt Output.txt

## 4.Step d: Commit them
To commit the staged files, use the following command: Before commit plese run the run the git init  command to initialize the git repository and also know status of  the repository using git status command
# Command..
git commit -m "Initial commit"

## 5.Step e: Push them to GitHub
Finally, to push the committed files to GitHub, use the following command Befor push plese create a repo on git hub and also  link your local repo to the remote repo
# Commands
git remote add origin https://github.com/your-username/your-repo-name.git
git push origin main

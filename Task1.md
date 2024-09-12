Based on what you have learnt in the class, do the following steps: 
1. a. Create a new folder 
2. b. Put the following files in the folder
                          Code.txt 
                          Log.txt 
                          Output.txt 
3. c. Stage the Code.txt and Output.txt files 
4. d. Commit them 
5. e. And finally push them to GitHub

## 1.Step a: Create a new folder
To create a new folder, you can use the command line interface (CLI) or your operating system's file explorer. Let's assume you're using the CLI. Open your terminal and type the following command
# Command..
1. mkdir myfolder

## 2.Step b: Put the following files in the folder
Create the following files inside the myfolder directory:
# Command..
1. cd myfolder
2. touch Code.txt Log.txt Output.txt

## 3.Step c: Stage the Code.txt and Output.txt files
To stage the Code.txt and Output.txt files, use the following Git commands:
# Command..
1. git add Code.txt Output.txt

## 4.Step d: Commit them
To commit the staged files, use the following command: Before commit plese run the run the git init  command to initialize the git repository and also know status of  the repository using git status command
# Command..
1. git commit -m "Initial commit"

## 5.Step e: Push them to GitHub
Finally, to push the committed files to GitHub, use the following command Befor push plese create a repo on git hub and also  link your local repo to the remote repo
# Commands
1. git remote add origin https://github.com/your-username/your-repo-name.git
2. git push origin main

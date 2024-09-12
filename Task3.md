Tasks to Be Performed: 
1. Create a Git working directory, with the following branches: 
               Develop 
               F1 
               f2 
2. In the master branch, commit main.txt file 
3. Put develop.txt in develop branch, f1.txt and f2.txt in f1 and f2 respectively 
4. Push all these branches to GitHub
5. On local delete f2 branch 
6. Delete the same branch on GitHub as well



## Task 1: Create a Git working directory with the following branches: Develop, F1, F2
To create a new Git repository, we can use the following command:
### Commond
1. git init
This will create a new Git repository in the current directory.
### Commond
Next, we can create the required branches using the following commands:
1. git branch Develop
2. git branch F1
3. git branch F2

## Task 2: In the master branch, commit main.txt file
First, let's create a new file called main.txt in the master branch:
### Command
1. echo "This is the main branch" > main.txt
Then, we can add and commit the file using the following commands:
### Command
2. git add main.txt
3. git commit -m "Initial commit on master branch"

## Task 3: Put develop.txt in develop branch, f1.txt and f2.txt in f1 and f2 respectively
Let's switch to the Develop branch and create a new file called develop.txt:
### Command
1. git checkout Develop
2. echo "This is the Develop branch" > develop.txt
3. git add develop.txt
4. git commit -m "Initial commit on Develop branch"

### Next, let's switch to the F1 branch and create a new file called f1.txt:
5. git checkout F1
6. echo "This is the F1 branch" > f1.txt
7. git add f1.txt
8. git commit -m "Initial commit on F1 branch"

### Finally, let's switch to the F2 branch and create a new file called f2.txt:
9. git checkout F2
10. echo "This is the F2 branch" > f2.txt
11. git add f2.txt
12. git commit -m "Initial commit on F2 branch"

## Task 4: Push all these branches to GitHub
First, we need to create a new repository on GitHub and add the remote repository to our local Git repository. Let's assume the repository URL is https://github.com/username/repository.git. We can add the remote repository using the following command:
### Command 
1. git remote add origin https://github.com/username/repository.git
### Next, we can push all the branches to GitHub using the following command:
2. git push --all origin

## Task 5: On local delete f2 branch
We can delete the F2 branch locally using the following command:
### Command
1. git branch -d F2

## Task 6: Delete the same branch on GitHub as well
We can delete the F2 branch on GitHub using the following command:
###   Command
1. git push origin --delete F2

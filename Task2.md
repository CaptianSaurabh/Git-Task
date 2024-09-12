Task: Please share the commands for the above point
 Tasks to Be Performed: 
1. Create a Git working directory with feature1.txt and feature2.txt in the master branch 
2. Create 3 branches develop, feature1 and feature2 
3. In develop branch create develop.txt, do not stage or commit it 
4. Stash this file and check out to feature1 branch 
5. Create new.txt file in feature1 branch, stage and commit this file 
6. Checkout to develop, unstash this file and commit 
7. Please submit all the Git commands used to do the above steps


# Task 1: Create a Git working directory with feature1.txt and feature2.txt in the master branch
## Command
1 mkdir myrepo
2 cd myrepo
3 git init
4 touch feature1.txt feature2.txt
5 git add .
6 git commit -m "Initial commit"

# Task 2: Create 3 branches develop, feature1, and feature2
## Command
1 git branch develop
2 git branch feature1
3 git branch feature2

# Task 3: In develop branch create develop.txt, do not stage or commit it
## Command
1 git checkout develop
2 touch develop.txt

# Task 4: Stash this file and check out to feature1 branch
## Command
1git stash
2git checkout feature1

# Task 5: Create new.txt file in feature1 branch, stage and commit this file
## Command
1 touch new.txt
2 git add new.txt
3 git commit -m "Added new.txt in feature1 branch"

# Task 6: Checkout to develop, unstash this file and commit
## Command 
1 git checkout develop
2 git stash pop
3git add develop.txt
4 git commit -m "Added develop.txt in develop branch"

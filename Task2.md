Task: Please share the commands for the above point
 Tasks to Be Performed: 
1. Create a Git working directory with feature1.txt and feature2.txt in the master branch 
2. Create 3 branches develop, feature1 and feature2 
3. In develop branch create develop.txt, do not stage or commit it 
4. Stash this file and check out to feature1 branch 
5. Create new.txt file in feature1 branch, stage and commit this file 
6. Checkout to develop, unstash this file and commit 
7. Please submit all the Git commands used to do the above steps


>>Task 1: Create a Git working directory with feature1.txt and feature2.txt in the master branch
mkdir myrepo
cd myrepo
git init
touch feature1.txt feature2.txt
git add .
git commit -m "Initial commit"

>>Task 2: Create 3 branches develop, feature1, and feature2
git branch develop
git branch feature1
git branch feature2

>>Task 3: In develop branch create develop.txt, do not stage or commit it
git checkout develop
touch develop.txt

>>Task 4: Stash this file and check out to feature1 branch
git stash
git checkout feature1

>>Task 5: Create new.txt file in feature1 branch, stage and commit this file
touch new.txt
git add new.txt
git commit -m "Added new.txt in feature1 branch"

>>Task 6: Checkout to develop, unstash this file and commit
git checkout develop
git stash pop
git add develop.txt
git commit -m "Added develop.txt in develop branch"
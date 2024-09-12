Tasks to Be Performed: 
1. Put master.txt on master branch, stage and commit 
2. Create 3 branches: public 1, public 2 and private 
3. Put public1.txt on public 1 branch, stage and commit 
4. Merge public 1 on master branch 
5. Merge public 2 on master branch 
6. Edit master.txt on private branch, stage and commit 
7. Now update branch public 1 and public 2 with new master code in private 
8. Also update new master code on master 
9. Finally update all the code on the private branch


#### Task 1: Put master.txt on master branch, stage and commit
First, let's create a new file called master.txt in the master branch:
### Command
1. echo "This is the master branch" > master.txt
2.Then, we can add and commit the file using the following commands:
3. git add master.txt
4. git commit -m "Initial commit on master branch"

#### Task 2: Create 3 branches: public 1, public 2 and private
We can create the required branches using the following commands:
### Command
1. git branch public1
2. git branch public2
3. git branch private

#### Task 3: Put public1.txt on public 1 branch, stage and commit
Let's switch to the public1 branch and create a new file called public1.txt:
### Command
1. git checkout public1
2. echo "This is the public1 branch" > public1.txt
3. git add public1.txt
4. git commit -m "Initial commit on public1 branch"

#### Task 4: Merge public 1 on master branch
Let's switch back to the master branch and merge the public1 branch:
### Command
1. git checkout master
2. git merge public1

#### Task 5: Merge public 2 on master branch
Since there are no changes on the public2 branch, we can simply merge it with the master branch:
### Command
1. git merge public2

#### Task 6: Edit master.txt on private branch, stage and commit
Let's switch to the private branch and edit the master.txt file:
### Command
1. git checkout private
2. echo "This is the updated master branch" > master.txt
3. git add master.txt
4. git commit -m "Updated master.txt on private branch"

#### Task 7: Now update branch public 1 and public 2 with new master code in private
We can merge the private branch with the public1 and public2 branches:
### Command
1. git checkout public1
2. git merge private
3. git checkout public2
4. git merge private

#### Task 8: Also update new master code on master
We can merge the private branch with the master branch:
### Command
1. git checkout master
2. git merge private

#### Task 9: Finally update all the code on the private branch
Since we've already merged the private branch with the master branch, we don't need to do anything else. The private branch is already up-to-date.


Here's a summary of the Git history:

A -- B -- C   (master)
|       \
|        D   (public1)
|       /
E -- F   (private)
 \
  G   (public2)

Where:
A: Initial commit on master branch
B: Merge public1 branch
C: Merge private branch
D: Initial commit on public1 branch
E: Initial commit on private branch
F: Updated master.txt on private branch
G: Initial commit on public2 branch

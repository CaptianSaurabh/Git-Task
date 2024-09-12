+
 *--++++++++++*------------------------------------*Tasks to Be Performed: 
1. Create a Git Flow workflow architecture on Git 
2. Create all the required branches 
3. starting from e feature branch, push the branch to the master, following the architecture 
4. Push an urgent.txt on master using hotfix


#### Task 1: Create a Git Flow workflow architecture on Git
Git Flow is a branching model for Git that helps to manage large projects. It consists of two main branches: master and develop. The master branch is used for production-ready code, while the develop branch is used for development.
To initialize Git Flow, we can use the following command:
### Command
1. git flow init
##### This will create the master and develop branches.

#### Task 2: Create all the required branches
In addition to the master and develop branches, we also need to create the following branches:
1.feature/: for feature branches
2.release/: for release branches
3.hotfix/: for hotfix branches
4.support/: for support branches
##### We can create these branches using the following commands:
5.git branch feature/
6.git branch release/
7.git branch hotfix/
8.git branch support/

However, in Git Flow, we don't create these branches manually. Instead, we use the git flow command to create them.

#### Task 3: Starting from a feature branch, push the branch to the master, following the architecture
##### Let's create a new feature branch called feature/new-feature:
1. git flow feature start new-feature
##### This will create a new branch called feature/new-feature and switch to it.
##### Let's add some code to the feature branch:
2. echo "This is a new feature" > new-feature.txt
3. git add new-feature.txt
4. git commit -m "Added new feature"
##### Now, let's finish the feature branch and merge it with the develop branch:
5. git flow feature finish new-feature
##### This will merge the feature/new-feature branch with the develop branch.
##### Next, let's create a release branch:
6. git flow release start v1.0
##### This will create a new branch called release/v1.0 and switch to it.
##### Let's merge the develop branch with the release/v1.0 branch:
7. git merge develop
##### Now, let's finish the release branch and merge it with the master branch:
8. git flow release finish v1.0
##### This will merge the release/v1.0 branch with the master branch.

#### Task 4: Push an urgent.txt on master using hotfix
##### Let's create a new hotfix branch:
1. git flow hotfix start urgent-fix
##### This will create a new branch called hotfix/urgent-fix and switch to it.
##### Let's add the urgent.txt file:
2. echo "This is an urgent fix" > urgent.txt
3. git add urgent.txt
4. git commit -m "Added urgent fix"
##### Now, let's finish the hotfix branch and merge it with the master branch:
5. git flow hotfix finish urgent-fix
##### This will merge the hotfix/urgent-fix branch with the master branch.

Here's a summary of the Git history:
A -- B -- C   (master)
|       \
|        D   (develop)
|       /
E -- F   (feature/new-feature)
 \
  G -- H   (release/v1.0)
   \
    I   (hotfix/urgent-fix)
Where:

A: Initial commit on master branch
B: Merge develop branch
C: Merge release/v1.0 branch
D: Merge feature/new-feature branch
E: Initial commit on feature/new-feature branch
F: Finish feature/new-feature branch
G: Initial commit on release/v1.0 branch
H: Finish release/v1.0 branch
I: Finish hotfix/urgent-fix branch

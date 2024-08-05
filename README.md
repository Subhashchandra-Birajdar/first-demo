# first-demo
This is my first Git Repository.
<br>
Author - Subhash Birajdar(MH)
<hr>
<p>Git</p>
         1. version control system 
         2. tool that helps too tract changes in code.
         o3. pen source, free and open source, fast and scalale

<p>uses:</p>
	1. track the history code
	2. collaboration

<h1.Github:</h1> 
                1. Website that allows developers to store and manage their code using Git.
                2. store and manage the code. 
                3. upload the folder( repository) , also we can others code and make clone also

-------
Create a new Repository - first-demo
make our first commit

changes mean commit in github ( first .add -> commit)

after installation git and github and visual studio 
we will configure the git

(local and global change)
git config --global user.name "My Name"
git config --global user.email "someone@gmail.com"
git config --list
(inside git there is git helper basically it stores the credential like user,email,password)
~ consider as root directory

coding process with Git code


<p>Clone & status</p>
clone - cloning a repository on our local machine(repository(remote) -> local(machine))
	git clone <- project some link ->
                        git clone https://github.com/Subhashchandra-Birajdar/first-demo.git
	  (also  we can use ssh)

cd means change directory
cd first-demo   (here we will go to that directory, first-demo)
ls  = it will show all files (here two file hidden and non hidden)
ls -a --> it will show hidden files

status - diplays the state of the code
	git status

once you modified you have to add

modified(tracked) 
mean git know this file(Readme.md)

untracked 
mean new files(index.file)

stages
file is ready to be commited

inmodified
unchanged

=== when we add file then it will go to stage then we will commit then it will be unchange.

add
             adds new or changed files in your working directory to the git staging area
            git add <--file name -->   (single record)
            git add .     (multiple records)

commit
	it is record of change
	git commit - m " some message"  (meaning message)                  

Push
	upload local repo content to remote repo
	git push origin main( Here origin mean github)
========
for new project
we have to add some commands like

init 
         used to create a new git repo
          git init
          git remote add origin <--link-->
          git remove -v (to verify remote)
          git branch (to check branch)
          git branch -M main(to rename branch)
         git push origin main
         git push -u origin main( for project only use git push )


branch
                project -feature 1(frontend)dev
                                feature 2(backend)
	          bug fix 3
           cd ..
           mkdir LocalRepo	        

to shift(move) another branch
git checkout <-branch name--> (to navigate)

create new branch
git checkout -b <--new branch name-->

to delete branch
git checkout -d <---branch name-->

merging code
way1
to compare commits,branches,files and more
	git diff <-branch name -->
to merge 2 branches
	git merge <-branch name-->

way2
 create a PR(pull request)

PULL Request
It lets you tell others about changes you'have pushed to a branch in a repository on GitHub.

PULL Command
git pull origin main
used to fetch and download from a remote repo and immeditely update the local repo to match that content.

Resolving Merge Conflict
An event that takes place when Git is unable to automatically resolve differences in code between two commits.
1) PR
2) Git merge

git merge main (feature to main) - in this we have to set manually which one shoud commit
accept current change(feature1  branch) (currently using)
or
Incoming change(main branch)
or
Accept Both changes(in different line)

===
Undling Changes

case 1: staged changes
	git reset <--file name-->
                      git reset

case 2 : commited changes (for one commit)
	git reset Head ~1 (latest commit0

case 3 : commited changes(for many commits)
	git reset <--commit hash(unique code)-->
	git reset --hard <--commit hash-->
git log == all commit

======
Fork
A fork is a new repository that shares code and visibility setting with the original "upstream" repository.
Fork is a rough copy.

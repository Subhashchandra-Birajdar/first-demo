# first-demo
This is my first Git Repository.
<br>
Author - Subhash Birajdar(MH)
<hr>
<p>Git</p>
         1. version control system <br>
         2. tool that helps too tract changes in code.<br>
         3. pen source, free and open source, fast and scalale<br>
<br>
<p>uses:</p><br>
	1. track the history code<br>
	2. collaboration<br>

<h1>Github:</h1> <br>
                1. Website that allows developers to store and manage their code using Git.<br>
                2. store and manage the code. <br>
                3. upload the folder( repository) , also we can others code and make clone also<br>

-------
Create a new Repository - first-demo<br>
make our first commit<br>

changes mean commit in github ( first .add -> commit)<br>

after installation git and github and visual studio <br>
we will configure the git<br>

(local and global change)<br>
git config --global user.name "My Name"<br>
git config --global user.email "someone@gmail.com"<br>
git config --list<br>
(inside git there is git helper basically it stores the credential like user,email,password)<br>
~ consider as root directory<br>

coding process with Git code<br>

<p>Clone & status</p><br>
<p>clone - cloning a repository on our local machine(repository(remote) -> local(machine))</p><br>
	git clone <- project some link -><br>
        git clone https://github.com/Subhashchandra-Birajdar/first-demo.git<br>
	  (also  we can use ssh)<br>

<p>cd means change directory</p><br>
cd first-demo   (here we will go to that directory, first-demo)<br>
ls  = it will show all files (here two file hidden and non hidden)<br>
ls -a --> it will show hidden files<br>

<h1>status - diplays the state of the code</h1><br>
	git status<br>

<p>once you modified you have to add</p><br>

<h1>modified(tracked) </h1><br>
mean git know this file(Readme.md)<br>

<h1>untracked</h1><br> 
mean new files(index.file)<br>

<h1>stages</h1><br>
file is ready to be commited<br>

<h1>inmodified</h1><br>
unchanged<br>

when we add file then it will go to stage then we will commit then it will be unchange.<br>

<h1>add</h1><br>
        adds new or changed files in your working directory to the git staging area<br>
            git add <--file name -->   (single record)<br>
            git add .     (multiple records)<br>

<h1>commit</h1><br>
	1. it is record of change<br>
	2. git commit - m " some message"  (meaning message) <br>                 

<h1>Push</h1><br>
	1. upload local repo content to remote repo<br>
	2. git push origin main( Here origin mean github)<br>

for new project<br>
we have to add some commands like<br>

<h1>init</h1><br> 
         used to create a new git repo<br>
          git init<br>
          git remote add origin <--link--><br>
          git remove -v (to verify remote)<br>
          git branch (to check branch)<br>
          git branch -M main(to rename branch)<br>
         git push origin main<br>
         git push -u origin main( for project only use git push )<br>


<h1>branch</h1><br>
                project -feature 1(frontend)dev<br>
                        feature 2(backend)<br>
	                 bug fix 3<br>
           cd ..<br>
           mkdir LocalRepo<br>	        

to shift(move) another branch<br>
git checkout <-branch name--> (to navigate)<br>

create new branch<br>
git checkout -b <--new branch name--><br>

to delete branch<br>
git checkout -d <---branch name--><br>

merging code<br>
<h2>way1</h2><br>
to compare commits,branches,files and more<br>
	git diff <-branch name --><br>
to merge 2 branches<br>
	git merge <-branch name--><br>

<h2>way2</h2><br.
 <p>create a PR(pull request)</p><br>

<h1>PULL Request</h1><br>
It lets you tell others about changes you'have pushed to a branch in a repository on GitHub.<br>

<h1>PULL Command</h1><br>
git pull origin main<br>
used to fetch and download from a remote repo and immeditely update the local repo to match that content.<br>

<h1>Resolving Merge Conflict</h1><br>
An event that takes place when Git is unable to automatically resolve differences in code between two commits.<br>
1) PR<br>
2) Git merge<br>

git merge main (feature to main) - in this we have to set manually which one shoud commit<br>
accept current change(feature1  branch) (currently using)<br>
or<br>
Incoming change(main branch)<br>
or<br>
Accept Both changes(in different line)<br>

<h1>Undling Changes</h1><br>

case 1: staged changes <br>
	git reset <--file name--><br>
                      git reset<br>

case 2 : commited changes (for one commit)<br>
	git reset Head ~1 (latest commit0<br>

case 3 : commited changes(for many commits)<br>
	git reset <--commit hash(unique code)--><br>
	git reset --hard <--commit hash--><br>
git log == all commit<br>

<h1>Fork</h1><br>
A fork is a new repository that shares code and visibility setting with the original "upstream" repository.<br>
Fork is a rough copy.<br>

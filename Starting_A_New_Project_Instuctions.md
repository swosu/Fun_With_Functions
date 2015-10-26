# Read Me File to start a program (This is what shows up bold):
	Example:  Fun_With_Functions_Project

1. Start Eclipse
2. Change the workspace to our thumbdrive
	: File> Switch Workspace> Other
3. Start a new project: Fun_With_Functions_Project
	: File> New> Java Project
		: Use default runtime environment, 
			then click finish.
4. Add a new class with our new
	project selected: Fun_With_Functions
	: File> New> Class
		: Name it, select the public static
			void main option and Finish.


# Now begin Git on the local machine and Git Hub on the remote.

1. Open the command prompt.
	:Start> search for cmd> Strike Enter.
2. Go to your project folder
	: E: to change to thumb drive
	: dir to list the directory
	: E:\>cd COMSC_1033_Workspace to change
		to the correct workspace.
	: E:\COMSC_1033_Workspace>cd Fun_With_Functions_Project
	:E:\COMSC_1033_Workspace\Fun_With_Functions_Project
		You should be able to see
		the src and bin folders.
: E:\COMSC_1033_Workspace\Fun_With_Functions_Project>dir
 Volume in drive E has no label.
 Volume Serial Number is CF21-6DC3

 Directory of E:\COMSC_1033_Workspace\Fun_With_Functions_Project

10/26/2015  09:11 AM    <DIR>          .
10/26/2015  09:11 AM    <DIR>          ..
10/26/2015  09:11 AM               402 .project
10/26/2015  09:11 AM    <DIR>          src
10/26/2015  09:11 AM    <DIR>          bin
10/26/2015  09:11 AM               232 .classpath
               2 File(s)            634 bytes
               4 Dir(s)   8,100,921,344 bytes free
3. git init to begin a new local repository.
: E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git init
Initialized empty Git repository in E:/COMSC_1033_Workspace/Fun_With_Functions_P
roject/.git/

4. git add . to add my materials.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git add .

5. git config our user name and email.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git config user.name "Jeremy
Evert"

E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git config user.email "jeremy
.evert@swosu.edu"

6. Start a browser of choice.
7. Go to Github: https://github.com/
8. Log into your personal account: https://github.com/login
9. Add a new repository
	: Name it, and make it public, but do not initilize your folder with a 
		read me file. That initilization makes your life harder.
	: Press "Create Repository"
10. Follow the online instructions on how to 
	…or push an existing repository from the command line

: git remote add origin https://github.com/jeremy-evert/Fun_With_Functions.git
: git push -u origin master

So go back to the command prompt, and then do the first line, after pressing enter
	do the second.

// below is the first line. It works without problem.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git remote add origin https:/
/github.com/jeremy-evert/Fun_With_Functions.git

// below is the second line. note that it had problems.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git push -u origin master
error: src refspec master does not match any.
error: failed to push some refs to 'https://github.com/jeremy-evert/Fun_With_Fun
ctions.git'


// here we tried again, and it still was not happy.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git remote add origin https:/
/github.com/jeremy-evert/Fun_With_Functions.git
fatal: remote origin already exists.

// Here we try again, and still not happy.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git push -u origin master
error: src refspec master does not match any.
error: failed to push some refs to 'https://github.com/jeremy-evert/Fun_With_Fun
ctions.git'

// but I wanted to test how unhappy this was, so I tried to keep moving.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git add .

// So I just stayed after it. note that add and commit did not complain. 
// these are for my local repository.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git commit -m "first commit"
[master (root-commit) 2bf56dd] first commit
 3 files changed, 79 insertions(+)
 create mode 100644 .classpath
 create mode 100644 .project
 create mode 100644 Starting_A_New_Project_Instuctions.md

// Now we try to git push again. We got a very useful message.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

// now we try the new command.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>git push --set-upstream origi
n master
Username for 'https://github.com': jeremy.evert@swosu.edu
Password for 'https://jeremy.evert@swosu.edu@github.com':
Counting objects: 5, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 1.39 KiB | 0 bytes/s, done.
Total 5 (delta 0), reused 0 (delta 0)
To https://github.com/jeremy-evert/Fun_With_Functions.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.

// and all is well.
E:\COMSC_1033_Workspace\Fun_With_Functions_Project>







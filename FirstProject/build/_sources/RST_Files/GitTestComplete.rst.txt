Documentation on GIT-Test Complete Integration
---------------------------------------------------------------------------------

1)	Go to Tools->Options
2)	Make sure that Git is downloaded and installed into the system
3)	Go to Source Control
4)	Select Git-Plugin option 
5)	Make sure that all the projects are closed while setting up Git-Plugin
6)	Open the Project suite file which is to be posted to Repository (ex-Azure which uses GIT)
7)	Right Click on the Project suite and select Source Control->Create Repository
8)	Select the Project Suite file path
9)	Right Click on the Project suite and select Source Control->Commit
10)	It shows all the untracked files and staged files, give an appropriate commit message and click on Commit
11)	Right Click on the Project suite and select Source Control->Push
12)	Into the command line give “-c core.askpass= git remote add <remote link name>(ex origin) <remote repository link> (https://vnaganikhila@dev.azure.com/vnaganikhila/GITAzurePractice/_git/GITAzurePractice)
13)	We can also add a branch on giving in the command line “-c core.askpass=git branch <new branch name>
14)	Right Click on the Project suite and select Source Control->Push
15)	Select the value for “Push To Remote Repository” e.g. (Origin i.e. remote repo link name)
16)	If it needed to be pushed to master, select the option “Push Current branch” and click on push
17)	If it needed to be pushed to specific branch give command line as -c core.askpass=git checkout <branch name>
18)	Once again go to push tab and it shows Current Local Branch as the branch name other than master and click on push 
19)	 Basic Branch Properties: A new branch automatically copies the files present in master and when a new push is done it uploads/Updates the changes in new branch
20)	 Common Recuring Error: Updates were rejected on another repository pushing at the same time: Sol: A forced push can be done but it overwrites all the existing changes and commits. For a forced push give command line as “-c core.askpass=git push -f <remote repo link name> <branch >
21)	 Git Pull: Right Click on the Project suite and select Source Control->Pull
22)	For Fetch: Select the branch name in the field “Remote Branch to pull” and click on fetch ->Ok
23)	For Pull: Select the branch name in the field “Remote Branch to pull “and click on OK Pull performs Fetch and Merge and updates the changes and a dialog box appears showing changes were done outside test complete, Click on Yes/Yes to All, the changes will be updated

# How To Use Git
It is created to show the use of Github commands.

---

## If we have Git Project on Github before
- If already a project exists on Github or another Git remote server, we should "clone" it to our local computer.
To clone it we must use the Https URL of the repo which can be taken from the green "Code" button on the repo main page.
-After creating suitable folder for you, open terminal there(can be used VSCode terminal) and use this command:  
`git clone [URL]`    
- Then you have a project on your local. After entering the downloaded folder directory, you can see all project files and
you can change the project files as you wish.

---

## If we have a Project on local computer without Git 
1. If we have project on local computer, we can create a Git repo and send project to Remote Git Server. To do this, 
firstly create an empty(even any file like readme,license shouldnot be included.) repo on Remote Git Server like Github. Then in local, we must be in the project root directory. Here, after opening cmd or terminal of VSCode, we should initialize Git with this command:  
`git init`
2. Then it is suggestable to create a Readme file with the name of "README.md" in your local project file. After creating this file, "add" this to local Git, this step change the "stage" of this file. It means this command prepares file to be followed in git:  
`git add README.md`
3. To specify the reason of the change on file, we should use "commit" because the the changes on the files are stored as history of the files.Actually, it is the aim of Git. It stores every stage of the files and commits are useful to understand changes on files. If we dont commit, we can not push our files to Git Server.  
`git commit -m "first commit"`
4. Project on Git has branches to work different subjects in our projects. For example, while Bugrahan is making A part of current project, Muhammet is making B part of current project. Not to affect each other, projects are divided into branches. 
Initially, there is only one branch. To rename it as "main", use it:  
`git branch -M main`
5. We should give the remoter Server adress to upload our project. Actually, we will assign the Remote Server URL to "origin"(think it as a constant which store URL address). To do this:  
`git remote add origin [URL]`
6. For final step, we will push the project on local to Git Remote Server(origin=URL,main is our fundamental branch). Then the project is accesible from online.  
`git push -u origin main`

---

## To use Git on your current project (after the steps above)
After creating your repo as above, you can change your codes or you can add new files to your project, anything like that, you will use these commands:
1. When any file is changed, "add" them to prepare file to send local repo. Use it:  
`git add <file name>`  
or `git add .` "." means "all files".
2. Give the information for change on file to follow later, so tell the stage of file to Git via "commit":  
`git commit -m "file is changed due to this reason ... `
3. Now the files are stored in your local Git, everything is okay in local, but the updated project files still doesnt exist Remote Server, github. So push them to Remote Server to store in online.  
`git push`   
Use these steps for the changes on your project.




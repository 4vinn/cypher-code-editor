### Deployed on Railway
 <br>
Its frontend railway service - https://4vinn-cypher.up.railway.app/ <br>
Its backend railway service - https://4vinn-cypher-be.up.railway.app/ <br>

<br><br>


Useful links: <br>

```
https://discord.com/channels/713503345364697088/1187120237947125910  <br>
https://chat.openai.com/share/405fc4b6-ee1b-49ba-a3a7-84ed640c568a  <br>
https://chat.openai.com/share/996d4d7c-8a60-4037-a4cd-b017fc0699c1
```

Git commands:

//push your project from VS Code to your GitHub repository:

- Navigate to the root directory of your project
- git inti (create a new repo)
- git add . (add all files in the current directory to staging area)
- git commit -m "Initial commit" (commit changes)
- git remote add origin https://github.com/4vinn/cypher-code-editor.git (now the repo we made using ```git init```, it will be connected to a remote repo made on github)
- git push -u origin main (push code from local branch to ```main``` branch of remote repo named ```origin```, ```-u``` short for ```--set-upstream```, once set, we can use ```git push, git pull``` without specifying remote and branch name, as it sets up tracking relationship)


//you did some chanegs in code file in ```app.js```
- git status (It provides information about changes that have been made, which files are currently staged for the next commit, and which files are not yet tracked by Git.)
- git add app.js (on stage)
- git commit -m "added app.js"
- git push origin main (in repo)

//pushed to repo, but u did changes through github web. Now to update it on local machine too: 
//update your local code with the latest changes from the remote main branch:
```
- git fetch 
- git merge origin/main
```
 OR

```- git pull origin main
```



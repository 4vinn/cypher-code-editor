### A real-time code editor made using React.js, Node.js, Express.js, Websocet.io

---

#### Deployed on Railway
<br>

>Made 2 parallel railway services, one serving the frontend and the other serving the backend

Its frontend railway service - https://4vinn-cypher.up.railway.app/ <br>
Its backend railway service  - https://4vinn-cypher-be.up.railway.app/ <br>

<br>

>For that, I restructured my repo into a monorepo, that looks like this:
```
.
├── .gitignore
├── README
├── frontend/
│   ├── public
│   ├── src
│   ├── package.json
│   └── package-lock.json
└── backend/
    ├── server.js
    ├── actions.js
    ├── package.json
    └── package-lock.json
```
<br>

> Created separate `package.json` for each backend and frontend, updated scipts/dependencies accordingly

> Now, The `package-lock.json` file is used by npm to lock down the versions of dependencies to ensure consistent builds across different environments.  <br> Regenerated the `package-lock.json` in each folder using `install --package-lock-only`.
<details> 
<summary> npm install: </summary>

When you run npm install:

1. It looks at your package.json file and installs the dependencies specified there.

1. If there's a package-lock.json file, it uses it to ensure that the exact versions of the dependencies are installed.

1. It creates or updates the node_modules folder in your project directory, which contains all the installed dependencies.

It also generates a package-lock.json file if one does not exist or updates it to reflect the current state of installed dependencies.

</details>

> Made a railway service named "Cypher Code Editor - Frontend". Set the root dir to /frontend. Connected the github repo. Setuped the service variables. Generated a domain.

> Made a railway service named "Cypher Code Editor - Backend". Set the root dir to /backend. Connected the github repo. Generated a domain. 

> On frontend service, set service variable to call the backend domain. 

---

<details>
<summary> Other links: </summary> 

<br>

```
https://discord.com/channels/713503345364697088/1187120237947125910 
```
```
https://chat.openai.com/share/405fc4b6-ee1b-49ba-a3a7-84ed640c568a  
```
```
https://chat.openai.com/share/996d4d7c-8a60-4037-a4cd-b017fc0699c1
```

</details>

#### hidden field with metadata 👇

<div class="meta_for_parser tablespecs" style="visibility:hidden">{"dataname":"environment","colvar":"varname","colval":"value"} carsada</div>

#### hidden field with metadata 👆
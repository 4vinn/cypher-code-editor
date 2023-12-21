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
<summary> `npm install` </summary>

Here's what npm ci does:

It reads the package-lock.json file to determine the exact versions of dependencies.
It installs the exact versions specified in the lock file without making any changes to the node_modules folder.
It does not update the package-lock.json file.

</details>

---















<details>
<summary> Useful links: </summary> 

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

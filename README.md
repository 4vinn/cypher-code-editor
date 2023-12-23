### A real-time code editor made using React, Node, Express, and Socket.io

---

#### Deployed on Railway

Made 2 Railway services, one serving the frontend and the other serving the backend.

**Its frontend railway service:** https://4vinn-cypher.up.railway.app/ <br>
**Its backend railway service:** https://4vinn-cypher-be.up.railway.app/ <br>

For that, I restructured my repo into a shared monorepo that utilizes npm workspaces, it looks like this:
```
.
├── .gitignore
├── README
├── package.json
├── package-lock.json
└── apps/
    ├── frontend/
    │   ├── public
    │   ├── src
    │   └── package.json
    └── backend/
        ├── Actions.js
        ├── server.js
        └── package.json
```

The `package.json` at the root of the repository contains specific scripts to build and or start each app.

Created separate `package.json` for each backend and frontend, updated scripts/dependencies accordingly.

The `package-lock.json` file is used by npm to lock down the versions of dependencies to ensure consistent builds across different environments.  <br> Regenerate the `package-lock.json` by running `npm install --package-lock-only`.

### Details

When you run npm install:

1. It looks at the `package.json` files in the `apps/*` folders and installs the dependencies specified there.

2. It creates or updates the `node_modules` folder in your project directory, which contains all the installed dependencies.

It also generates a package-lock.json file if one does not exist or updates it to reflect the current state of installed dependencies.

### Deploying to Railway

1. Make an empty project
2. Add two empty services
3. Name one `Frontend`, name the other `Backend`
4. Generate domains for both services
5. On the `Frontend` service<br>
    Add these service variables:
    ```
    CI=false
    NIXPACKS_CONFIG_FILE=apps/frontend/nixpacks.toml
    REACT_APP_BACKEND_URL=https://${{Backend.RAILWAY_PUBLIC_DOMAIN}}
    ```
    Set the start command to: `npm run start:frontend`<br>
    Set the build command to: `npm run build:frontend`
6. On the `Backend` service<br>
    Set the start command to: `npm run start:backend`
7. Connect your GitHub repository to the `Backend` service
8. Connect the same Github repository to the `Frontend` service

**Notes**
- Leave each services root directory set to `/`

---

<details>
<summary> Other links: </summary> 

<br>
_hidden_

<!--
```
https://discord.com/channels/713503345364697088/1187120237947125910 
```
```
https://chat.openai.com/share/405fc4b6-ee1b-49ba-a3a7-84ed640c568a  
```
```
https://chat.openai.com/share/996d4d7c-8a60-4037-a4cd-b017fc0699c1
```
-->

</details>


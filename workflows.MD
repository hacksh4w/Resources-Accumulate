# CLI- CMD workflow
<br>

# How to create frontend and backend for a full stack app from initialization using Vite 

FRONTEND 
- cd into Frontend
- npm create vite@latest 
- . for same directory, or any name
- JS  + WSC
- npm i
- npm run dev


BACKEND 
- mkdir backend
- cd into Backend
- create server.js
- npm i express   //- npm init -y; to create package .json
- npm install -g nodemon / npm install --save-dev nodemon
- in package .json
"scripts": {
  "start": "nodemon server.js"
}
- npm start

## Initializing a git file (usual cmd commands not mentioned) => assume already logged into to Git

- make the files and usual shebang
    git init -b main // to initialise
    git add .
    git commit -m "first commit " // commits git locally 

// now for pushing to gh
- manually create a repo of reqd name
- dont create readme or uplaod any files
- copy repo url
    git remote add origin url
    git remote -v
    git push origin main
- now we're good to go



Note : the error `fatal: The current branch main has no upstream branch`.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.



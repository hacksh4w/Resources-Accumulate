# CLI- CMD workflow

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

# Initializing a git file (usual cmd commands not mentioned) => assume already logged into to Git

Mmake the files and usual shebang.
To Initialize a new branch, main, in the repository 
	
	git init -b main
  	
TO add all files : 

	git add . 
  	
git commit -m "first commit " 
// commits git locally 

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

# How to write Git commit messages? 
- *Content*: Be direct, try to eliminate filler words and phrases in these sentences (examples: though, maybe, I think, kind of). Think like a journalist
- *Mood*: Use imperative mood in the subject line. Example – Add fix for dark mode toggle state. Imperative mood gives the tone you are giving an order or request.
- *Length*: The first line <= 50 characters, and the body <= 72 characters.

- *Type of Commit*: Specify the type of commit; use consistent set of words to describe changes. 
	Example: Bugfix, Update, Refactor, Bump ...

The commit type can include the following:

- feat – a new feature is introduced with the changes
- fix – a bug fix has occurred
- chore – changes that do not relate to a fix or feature and don't modify src or test files (for example updating dependencies)
- refactor – refactored code that neither fixes a bug nor adds a feature
- docs – updates to documentation such as a the README or other markdown files
- style – changes that do not affect the meaning of the code, likely related to code formatting such as white-space, missing semi-colons, and so on.
- test – including new or correcting previous tests
- perf – performance improvements
- ci – continuous integration related.
- build – changes that affect the build system or external dependencies.
- revert – reverts a previous commit.


Examples  :
` feat : add search bar functionality`
`docs : add proj desc, abstract, hosted link `

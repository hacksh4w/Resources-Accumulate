# CLI- CMD workflow

## Table of Contents
1. [Initializing a git repo & pushing](#Git-Commands)
2. [How to create frontend and backend for a full stack app from initialization using Vite ](#Initialize-Full-Stack-App)
3. [How to write Git commit messages?](#Commit-Messages)

# Git Commands
## Initializing a git repo & pushing 
( assumption : already logged into to Github )

Make the files and usual things
To Initialize a new branch, main, in the repository type the following in ur terminal
	
	git init -b main
  	
To add all files : 

	git add . 
  	
Commits git locally in your PC

	git commit -m "first commit " 

####  now for pushing to gh
Manually create a repo of reqd name in github.com in your account
Note : do not create readme or upload any files 
Copy repo url that github.com generate's for you

	git remote add origin url

To check ur remote branch (it shud say main)

	git remote -v

Now to push all ur files and changes to the main branch of your remote repository

	git push origin main

And, now we're good to go!

Note : the error `fatal: The current branch main has no upstream branch`.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


# Initialize Full Stack App
## How to create frontend and backend for a full stack app from initialization using Vite 

## FRONTEND 
Make frontend Repository

	mkdir frontend

Move inside the frontend directory/folder : (. for same directory, or any name)

	cd frontend    

Run the following vite command to initialize vite

	npm create vite@latest 

- choose JS  + WSC in the options 
- mention your preferred name

Perform the following command to install all the files

	npm i

Perform the following command to run localhost server of your site

	npm run dev

## BACKEND Process
	
	mkdir backend

cd into Backend

	cd backend

Create `server.js` file
	
	npm i express   //- npm init -y; to create package .json

Install nodemon 

	npm install -g nodemon / npm install --save-dev nodemon

In your `package .json` file add

`"scripts": {`
 ` "start": "nodemon server.js"`
`}`

Then run the following to start server

	npm start
# Commit Messages
## How to write Git commit messages? 
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

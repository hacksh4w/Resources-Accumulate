# CLI- CMD workflow


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

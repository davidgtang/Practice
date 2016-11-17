# Basic stuff
A quick guide to git.
https://git-scm.com/book/en/v2

## Staging, Status of Changes
`git status`
Shows what you've edited, staged, etc.

`git add` 
Stage a file to be comitted. Any changes made after adding don't get committed.

`git status -s`
A shorter, compact version of `status`.

There are *2* columns. Left hand side indicates status of staging area, right hand column indicates status in working tree.
```
?? blah.txt (Untracked)
 M Readme   (Modified but not staged)
M  file2    (Modified and staged)
MM file3    (Staged one version, then changes made that are unstaged)
A  file4    (Adde new file)
```

`git diff`
Show changes that are unstaged.

`git diff --staged`
Changes in stage that will go into next commit.

## Committing
After adding stuff, `git commit` to finalize.

`-v`
Comments showing changes

`-a`
Skips the "add" stage. Adds everything for you.

See tutorials for how to undo changes.

## Remotes
`git remote -v`
Shows all remotes.

`git remote add <shortname> <url>`
Add additional remotes to folder.

`git fetch <shortname>`
To update from the remote

All fetch does is pull data down from repository, it doesn't merge any changes.

`git pull` on the other hand, does try and merge changes.

To push to remotes:
`git push [remote name][branch]`  
Example: `git push origin master`

`git remote show [remote-name]`
Used to show information about the remote.

## Tag section
Info coming later...

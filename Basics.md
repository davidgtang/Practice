# Basic stuff

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
##
`git diff`
Show changes that are unstaged.

`git diff --staged`
Changes in stage that will go into next commit.

## Committing
After adding stuff, commit `-v-`

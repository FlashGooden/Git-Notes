# Git

Git has 3 object types: Commit ---- Tree ----- Blob
  Commit contains the Author, Message, and a pointer to a tree of changes

  The tree contains pointers to file names, content and other trees

  The Blob contains data  (Source code, pictures, videos)

  Git add -p for a way to progressively see the file changes you are staging

# regular git commands
Rebasing

`git pull --rebase`

`git rebase --continue`

`git log --show-signature`

`git log -S 'getSingleGem'`

`git diff --cached` if you want to see the diff with the staged files

` git --no-pager log --oneline -5`  - shows 5 last commits in a log that doesn't open a new window

`git --no-pager log --graph` - shows a full graph of history and branches with comments

`git commit -a` adds the repo and lets you commit right away

`git push --force-with-lease` - Use when you need to push up to a feature branch, but you don't want to erase the changes someone will be making on their branch.

`git for-each-ref --sort=-committerdate --count=10 --format='%(refname:short)' refs/heads/` - shows the last 10 branches you checked out
`git rb` shortcut made using the above line in the github alias file



`git diff` shows changes on file

`git commit -am` commits file that was already added  and does message

`git reset HEAD~1` will reset the staged commit to the last current HEAD

git reset <hash> will reset to the staged commit

`git reset --hard HEAD^ ` hard resets to last commit

git reset --hard will reset and remove the commits from git

git add -p if you want to slowly go through your file changes hunk by hunk

type gp anywhere in github to see your open pull requests
type t to search for any file on a repo while in github

## git branch

`git branch --sort=-committerdate -a ` shows all the remote and local repo in order of commit DESC

  ## git stash
    git stash - will stash the file for you to retrieve

    git stash list  - will show you all the stashed files

    git stash show stash@{0} - will show you the stashed files

    git stash apply - will apply the last stash

    git stash apply stash@{0} - will apply a specific stash from the list

    git stash --all - WILL STASH ALL FILES INCLUDING YOUR .GITIGNORE

    git stash save "named stash" - Names a stash for easy reference

    git stash branch <optional branch name> - Starts a new branch from a stash

     git checkout <stash-name> <file-name> - checkout a certain file in a stash



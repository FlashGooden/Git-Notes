# Git 

Git has 3 object types: Commit ---- Tree ----- Blob
  Commit contains the Author, Message, and a pointer to a tree of changes

  The tree contains pointers to file names, content and other trees

  The Blob contains data  (Source code, pictures, videos)

  Git add -p for a way to progressively see the file changes you are staging 

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



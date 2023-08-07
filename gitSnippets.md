# Useful Git commands

### Cloning a repo
`git clone ssh://domain.com/path/project/project.git`

### Branching repo
`git checkout -b feature/new-local-branch`

### Commit changes
`git commit -S -a -m "initial commit to local branch"`

### Revert specific file to before changes
`git checkout HEAD^ -- path/to/file.ext`

### Push local branch to a new remote branch
`git push --set-upstream origin feature/new-remote-branch`

### Pull changes from remote branch
`git pull`

### Push local branch to existing remote branch
`git push -f`

### Delete local branch
`git branch -d feature/branch`

### Delete remote branch
`git push origin --delete feature/remote-branch`

### Make and no-edit commit
`git commit --amend --no-edit`

### Stash away current changes
`git stash push`

### Apply stashed away changes to current branch
`git stash pop`

### Save current changes to a file
`git stash clear; git stash push; git stash show "stash@{0}" -p > issue_ref.patch`

### Apply patch file to repo
`git apply issue_ref.patch`

### Create a patch from current branch
`git diff master branch > path/to/patch.patch`

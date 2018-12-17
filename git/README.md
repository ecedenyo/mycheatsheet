## Content: Git

* [Logs](#getting-log-information)
* [Tagging](#tagging)
* [Working with remotes](#working-with-remotes)

## Getting log information

- Main command: `git log`
- *oh-my-zsh* alias: `glo`
- Full command: `git log --oneline --decorate --color`

Next some daily-basis command options and their possible usages:

Command (*oh-my-zsh* alias) | Description
--- |--- 
`glo` | Show only a partial prefix commit (more readable) with its message
`glo -5` | Show the 5 recent commits (in more readable mode)
`glo --before=2018-10-01` | Show only commits (in readable mode) done before the specified date
`glo --no-walk --tags` | Show only tagged commits (in more readable mode)

## Tagging

- Main command: `git tag`
- *oh-my-zsh* alias: -
- Full command: -

Next some daily-basis command options and their possible usages:

Command | Description
--- | --- 
`git tag mytag 4da45be` | Tag _(lightweight, simplest mode)_ a specified commit
`git tag` | List all created tags in the repo
`git tag -l "v1.7*"` | List all created tags in the repo matching given (kindda) pattern
`git describe` | List only all **annotated** tags in the repo
`git tag -a mytag 4da45be -m "My message"` | Associate to a commit (ID specified) a given tag
`git tag -d mytag` | Drop the specified tag, doesn't affect possible related commits
`git show mytag` | Show information saved when (annotate) tagging and related to the commit associated

## Working with remotes
Command (*oh-my-zsh* alias) | Description
--- | --- 
`ggpull` | **Pull** from origin to current branch
`ggpnp` | **Pull** from origin (to current branch) and **push** to origin (from current branch) in one operation (if no merges are necessary)
`ggp` | **Push** to origin from current branch
`gpoat` | Push *all (branches)* and *tags* to origin


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExNjczMzIzOTUsLTEwNjI2MTUzODAsLT
E4NjA2NTg3NjBdfQ==
-->

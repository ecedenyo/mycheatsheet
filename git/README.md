## git commands - Content

* [Logs](#logs)
* [Tagging](#tagging)

## Logs

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
`git tag mytag 4da45be` | Tag (simplest mode) a specified commit
`git tag -l` | List all created tags in the repo
`git tag -a mytag 4da45be -m "My message"` | Associate to a commit (ID specified) a given tag
`git tag -d mytag` | Drop the specified tag, doesn't affect possible related commits
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTY1OTM1NTk0OCwtMTA2MjYxNTM4MCwtMT
g2MDY1ODc2MF19
-->
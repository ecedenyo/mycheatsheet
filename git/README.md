## git commands - Content

* [Logs](#logs)
* [Tagging](#tagging)

## Logs

- Main command: `git log`
- : 
- Full command: `git log --oneline --decorate --color`

Next some daily-basis command options and their possible usages:

*oh-my-zsh* alias | Description
--- |--- 
`glo` | Show only a partial prefix commit (more readable) with its message
`glo -5` | Show the 5 recent commits (in more readable mode)
`glo --before=2018-10-01` | Show only commits (in readable mode) done before the specified date
`glo --no-walk --tags` | Show only tagged commits (in more readable mode)

## Tagging
Main command | Main oh-my-zsh alias (omza) | (omza) full command
--- | --- | --- 
`git tag` | `---` | `---`

Next some daily-basis command options and their possible usages:

Command options | (Short) full command / </br>(Possible) Usage | Description
--- | --- | ---
`---` | `git tag mytag 4da45be` | Tag (simplest mode) a specified commit
`-l`, `--list` | `git tag -l` | List all created tags in the repo
`-a` | `git tag -a mytag 4da45be -m "My message"` | Associate to a commit (ID specified) a given tag
`-d` | `git tag -d mytag` | Drop the specified tag, doesn't affect possible related commits
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1NDc5NDQwMTksLTEwNjI2MTUzODAsLT
E4NjA2NTg3NjBdfQ==
-->
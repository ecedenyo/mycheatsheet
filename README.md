# myguide: git commands
Daily-basis git commands 

## Content
* [Logs](#logs)
* [Tagging](#tagging)

---

## Logs
Main command | Main oh-my-zsh alias (omza) | (omza) full command
--- | --- | --- 
`git log` | `glo` | `git log --oneline --decorate --color`

Next some daily-basis command options and their possible usages:

Command options | (Short) full command / </br>(Possible) Usage | Description
--- | --- | ---
`--oneline` | `glo` | Show only a partial prefix commit (more readable) with its message
`-5` | `glo -5` | Show the 5 recent commits (in more readable mode)
`--before=2018-10-01` | `glo --before=2018-10-01` | Show only commits (in readable mode) done before the specified date
`--no-walk --tags` | `glo --no-walk --tags` | Show only tagged commits (in more readable mode)

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

---

# WP CLI

## Theming
Main command | Description
--- | --- 
`wp theme list status=active` | Show active theme

## Plugins
Main command | Description
--- | --- 
`wp plugin list` | Get list of installed plugins
`wp plugin activate my_plugin` | Activate plugin my_plugin
`wp plugin deactivate my_plugin` | Deactivate plugin my_plugin

---

# MySQL

Main command | Description
--- | --- 
`show columns from <table> like '%person%'` | Show columns that match the given criteria (i.e. partial column name includes 'person')

# myguide: git commands
Daily-basis git commands 

## Logs
Main command: `git log`

Command options | Short full command / </br>(Possible) Usage | Description
--- | --- | ---
`--oneline` | `glo` | Show only a partial prefix commit (more readable) with its message
`-5` | `glo -5` | Show the 5 recent commits (in more readable mode)
`--before=2018-10-01` | `glo --before=2018-10-01` | Show only commits (in readable mode) done before the specified date
`--no-walk --tags` | `glo --no-walk --tags` | Show only tagged commits (in more readable mode)

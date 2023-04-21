# Contributing

## Merge Requests (MR) or Pull Requests (PR)

- MRs or PRs are mandatory to apply technical validation(s)
- Each change requires a single MR or PR in respect of branches and commit rules
- If an open thread is present, merge button won't be available: you have to process returns
- Only when a MR or PR is twice validated (condition can be overruled by experts) developer can apply it
- Ticketing system MUST be up-to-date according to MR status

## Branches

```
<type>-<ticketing-id>
```

With:

- `<type>`: see next chapter
- `<ticketing-id>`: ticketing system id (example: 666)

## Commits

From namings :

- https://dev.to/i5han3/git-commit-message-convention-that-you-can-follow-1709
- http://karma-runner.github.io/1.0/dev/git-commit-msg.html
- https://www.conventionalcommits.org/en/v1.0.0/#specification

Base template

```
<type>(<scope>): <subject>

<body>

<footer>
```

Allowed `<type>` values:
- **feat** (new feature for the user, not a new feature for build script)
- **fix** (bug fix for the user, not a fix to a build script)
- **build** (build related changes like adding external dependencies)
- **chore** (updating grunt tasks etc.; no production code change)
- **docs** (documentation related changes)
- **style** (formatting, missing semi colons, etc; no production code change)
- **refactor** (refactoring production code, eg. renaming a variable)
- **test** (adding missing tests, refactoring tests; no production code change)
- **perf** (performance improvement code)


Example `<scope>` values (could be anything specifying place of the commit change):
- init
- config
- cron
- cli
- ci-cd
- exec
- images
- *...*

CLI example: 

```
git commit -m "feat(cli): add customer email lambda notification" -m "" -m "Fixes #666"
```

Empty line is mandatory

`Fixes #666` having #666 your ticketing system ID is also mandatory

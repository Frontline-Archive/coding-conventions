# Commit Messages

## The reasons for these conventions:
- automatic generating of the changelog
- simple navigation through git history (eg. ignoring style changes)

## Format of the commit message:
```bash
<type>(<scope>): <subject>

<body>

<footer>
```


## Message subject (first line)
First line cannot be longer than 70 characters, second line is always
blank and other lines should be wrapped at 80 characters.

### Allowed `<type>` values:

* **feature** (new feature for the user, not a new feature for build script)
* **fix** (bug fix for the user, not a fix to a build script)
* **docs** (changes to the documentation)
* **style** (formatting, missing semi colons, etc; no production code change)
* **refactor** (refactoring production code, eg. renaming a variable)
* **test** (adding missing tests, refactoring tests; no production code change)
* **chore** (updating grunt tasks etc; no production code change)

### Example `<scope>` values:

* init
* runner
* watcher
* config
* web-server
* proxy
* etc.

The `<scope>` can be empty (eg. if the change is a global or difficult
to assign to a single component), in which case the parentheses are
omitted.


## Message body
* uses the imperative, present tense: “change” not “changed” nor “changes”
* includes motivation for the change and contrasts with previous behavior

For more info about message body, see:

* http://365git.tumblr.com/post/3308646748/writing-git-commit-messages
* http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html


## Message footer

### Referencing issues
Closed issues should be listed on a separate line in the footer prefixed with "Closes" keyword like this:
```bash
Closes 234
```
or in case of multiple issues:
```bash
Closes 123, 245, 992
```
To enable auto-linking to issues created in GitHub prefix the issue number with "#" like this:
```
Closes #583
```

# Branching Strategy
![Branching Strategy](https://github.com/fakewaffle/coding-conventions/raw/master/images/git-branching-model.png)

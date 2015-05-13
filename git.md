# Commit Messages

## The reasons for these conventions:
- automatic generating of the changelog
- simple navigation through git history (eg. ignoring style changes)
- understandable git [history](#git-history)

## Format of the commit message:
```
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
* **release** (updating package version numbers for a release)

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
Issues should be listed on a separate line in the footer prefixed with either a "Closes" or "Issue(s)" keyword. "Closes" should be used for issues that are completed. If it is a large issue and the commit only addresses part of the issue you should reference the issue with "Issue(s)" like this:
```bash
# Closed Issue
Closes 234

# Referenced Issue
Issue 234
```
or in case of multiple issues:
```bash
# Closed Issues
Closes 123, 245, 992

# Referenced Issues
Issues 123, 245, 992
```
To enable auto-linking to issues created in GitHub prefix the issue number with "#" like this:
```bash
# Closed Issue
Closes #583

# Referenced Issue
Issue #583
```

# Git History
The beauty of working with version control, such as Git, is the ability to see the history of things that have happened. It is very easy to ruin some of those benefits by making the history messing with unnecessary merge commits.

Without rebasing

```
* een0p3b - fix: implement awesome
*   9cn0p31 - Merge pull request #3
|\
| * 4dn0p31 - chore: add file
* |   83n0p38 - Merge pull request #2
|\ \
| |/
| * cbn0p30 - chore: do stuff
|/
*   6an0p34 - Merge pull request #1
|\
| * e3n0p3c - feature: new feature
|/
* 41n0p38 - chore: initial commit
```

With rebasing

```
* een0p3b - fix: implement awesome
* 4dn0p31 - chore: add file
* cbn0p30 - chore: do stuff
* e3n0p3c - feature: new feature
* 41n0p38 - chore: initial commit
```

This example is nearly a 40% reduction in commits by simply removing unnecessary merge commits. Sometimes it is advantageous to add merge commits, e.g. when merging in a long running feature branch. That way all the merge commits stay together.

```
*  4by3s0f - merge branch 'new-feature' into dev
|\
| * ddy3sa3 - feature(new-feature): update edivation training link to login
| * 6by3sa9 - feature(new-feature): prevented closed caption menu from showing with the new videojs version.
* | 3fy3s9c - fix: share icon event on user-uploaded segment cards
* | 3ey3s2e - fix: defect #6350 ios share results blocked
| * 3ay3sd9 - feature(new-feature): use version of backbone.touch that supports touch + mouse devices
| * f0y3s87 - fix(new-feature): ie 9 css rules limit.
| * b7y3s0c - fix(new-feature): caching swf until after embedding has completed
| * 87y3s89 - feature(new-feature): implemented relevance switching on clear filters.
* | 6by3sb3 - fix: defect regarding error message appearing when navigating from different groups page tabs to groups list
* | 11y3s86 - feature: updated videojs version to 4.6.4 and added videojs errors plugin.
* | 72y3sd4 - fix: reflection questions height to show autosave text
```

# Branching Strategy
![Branching Strategy](https://github.com/fakewaffle/coding-conventions/raw/master/images/git-branching-model.png)

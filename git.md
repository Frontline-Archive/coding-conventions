## Commit Messages
From [the git documentation](http://git.kernel.org/cgit/git/git.git/tree/Documentation/SubmittingPatches?id=HEAD)
* provide a meaningful commit message
* use past tense: "Changed" or "Changes", not "Change". (This differs from the documentation which uses imperative, present tense)
* If applicable, reference the story or task # in the title (and in the bullet items where appropriate).
    * Don't use a hash (#) in front of the story or it will link to github issues
* If applicable, reference an github issue using a hash (#) and the number
    * e.g. `#45`
    * With the correct verbs, this will close issues automatically.

Commit messages should be formatted as follows:

```
Added support for IE5 (52)

- Changed all Array.forEach to _.each()
- Refactored the Goblin class (142)
```

## Branching Strategy
![Branching Strategy](https://github.com/fakewaffle/coding-conventions/raw/master/images/git-branching-model.png)

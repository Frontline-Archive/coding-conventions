## About

We each play an important role in the success of the products we build in both the short and long term. When development groups are small and limited to just a few individuals, who often work in silos, refactoring, maintaining, and extending our code is easy; we wrote it and intimately know it! However, this becomes a challenge in a larger group, as each developer on a team, and each team will have their own conventions and standards. Conventions include file organization, indentation, comments, declarations, statements, white space, naming conventions, programming practices, programming principles, programming rules of thumb, architectural best practices, etc.

Much of our development time is spent reading code and exploring a project. This is especially true when a project is completed and falls into maintenance, we are fixing bugs, or working on projects we did not create. We read code to understand a project, to find patterns so we can refactor, to find bugs, etc. Most of our time is spent reading code!

Early on in the development of the new platform, we recognized the need for consistency. A lot of time was spent on developing coding conventions and project standards. If conventions are mixed throughout a project or between projects, it affects the readability and ease of understanding. It’s understood that not every standard chosen is the easiest to implement, but they meet the goals of maintainability, readability, extendability and familiarity. Some people may feel that the particular style or standard is wrong, but it should be followed because consistency is far more important.

As an organization, we need to write code for humans and not machines.

### Coding Conventions and Standards
* [git](https://github.com/sinet/coding-conventions/blob/master/git.md)
* [npm](https://github.com/sinet/coding-conventions/blob/master/npm.md)
* [JavaScript](https://github.com/sinet/coding-conventions/blob/master/javascript.md)
* [HTML](https://github.com/sinet/coding-conventions/blob/master/html.md)
* [CSS / Less](https://github.com/sinet/coding-conventions/blob/master/css.md)
* [iOS](https://github.com/sinet/coding-conventions/blob/master/ios.md)

### Additional Reading
The following three books are great reference for this topic. It is highly recommend that everyone read them:
* [The Art of Readable Code](http://shop.oreilly.com/product/9780596802301.do)
* [Code Simplicity](http://shop.oreilly.com/product/0636920022251.do)
* [Code Complete (2nd Edition)](http://www.amazon.com/Code-Complete-Practical-Handbook-Construction/dp/0735619670)

## Setup / Configuration
For new or uninitialized projects, use terminal to download the following linting and editor configuration files in your project directory:
```bash
curl -O https://raw.githubusercontent.com/sinet/coding-conventions/master/.editorconfig
curl -O https://raw.githubusercontent.com/sinet/coding-conventions/master/.eslintrc
```

Install the following packages for your editor/IDE of choice:

| Sublime Text 3 |  Atom [0] |
| :------------: | :--: |
| [EditorConfig](https://github.com/sindresorhus/editorconfig-sublime) | [EditorConfig](https://atom.io/packages/editorconfig) |
| [SublimeLinter](https://github.com/SublimeLinter/SublimeLinter3) | [Linter](https://atom.io/packages/linter) |
| [SublimeLinter-eslint](https://github.com/roadhump/SublimeLinter-eslint) | [linter-eslint](https://atom.io/packages/linter-eslint) |
| ? | [other linters (e.g. htmlhint, stylelint)](http://atomlinter.github.io/) |
| [DocBlockr](https://github.com/spadgos/sublime-jsdocs) | [DocBlockr](https://atom.io/packages/docblockr) |

[0] With Atom the following should be able to be installed directly from the command line, via:
```
apm install editorconfig linter linter-eslint docblockr
```

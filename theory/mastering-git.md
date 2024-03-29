---
competencies:
- git-3
---

# Mastering git

By now, you mastered git branching and the workflows, how can you use branching efficiently. Now, let's learn some extra stuff to really master git!

## Cool features of git

### Amend your last commit

Git has a number of awesome features; Not least of all is the ability to amend the previous commit. If you ever find that you accidentally left something out of your last commit, be it a file or an extra change to a file that you just committed, don't worry. It can easily be fixed

All you have to do is stage the extra changes like you would for a normal commit:

`git add .`

And then just commit with the `--amend` argument.

`git commit --amend`

If you don't specify a commit message with `-m` you will be prompted with the previous commit message as a default.

### Referencing commits

In order to understand the following features, you have to understand how you can refer to commits already made.

Please read and understand the following article about references:

<https://git-scm.com/book/en/v2/Git-Tools-Revision-Selection>

Okay-okay, we hear your voice, it's not that understandable, right?

Please finish _Main/Ramping up_ from the following interactive tutorial, what will definitely help in understanding!

<http://learngitbranching.js.org>

### Log

Please read and understand the following articles about git log:

<https://www.atlassian.com/git/tutorials/inspecting-a-repository/git-log>

<https://www.atlassian.com/git/tutorials/git-log/filtering-the-commit-history>

### Diff

Please read and understand the following articles:

<http://veerasundar.com/blog/2011/06/git-tutorial-comparing-files-with-diff/>

### Cherry-picking

Please read and understand the following articles:

<http://think-like-a-git.net/sections/rebase-from-the-ground-up/cherry-picking-explained.html>

Please finish _Main/Moving work around/Cherry pick intro_ from the following interactive tutorial:

<http://learngitbranching.js.org>

### Stashing

Please read and understand the following article:

<https://git-scm.com/book/en/v1/Git-Tools-Stashing>

### Handling remotes

Please finish all steps from the _Remote/Push & Pull -- Git Remotes!_ section of the following tutorial:

<http://learngitbranching.js.org>

## If something is still not clear...

It's really important to understand all the things listed above. If you still uncertain using some of the features, please try the following tutorials:

<https://www.git-tower.com/learn/git/ebook/en/mac/introduction> (you can change between Desktop and Command line)

<https://backlogtool.com/git-guide/en/>

<https://git-scm.com/documentation/external-links>

<https://www.atlassian.com/git/>

In case you found anything not listed here, please let the others know about it in the relevant discussion.

Git's UI is not really self-explanatory, and it's hard to forget the commands. You can print and use the official cheat-sheet, whenever you need it:

<https://github.com/github/training-kit/blob/master/downloads/github-git-cheat-sheet.pdf>

## Extra

If you have some extra time, please finish all unfinished sections from the Git branching tutorial:

<http://learngitbranching.js.org>

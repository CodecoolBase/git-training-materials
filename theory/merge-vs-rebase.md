---
competencies:
- git-3
---

# Git merge vs rebase

We have used `git merge` a lot by now, we know that with `git merge master` will merge the `master` branch into our currently checked out branch. That is nice, but what is this `git rebase`?

Rebasing is the process of moving commits to a new base commit. For example if we move the two commits of the `Feature` branch to the `Master` branch we could visualize it like this:

![gitrebase](../images/rebase.svg)

Hmm.. modifying the git history? Isn't that dangerous?

>The `git rebase` command has a reputation for being magical Git voodoo that beginners should stay away from, but it can actually make life much easier for a development team when used with care.

So it can be dangerous, but there is only one very important rule you have to keep in mind, they call it the "[The Golden Rule of Rebasing](https://www.atlassian.com/git/tutorials/merging-vs-rebasing#the-golden-rule-of-rebasing)":

> The golden rule of git rebase is to never use it on public branches.
> (You should never rebase commits once they've been pushed to a public repository.)

There is a great article about the topic by atlassian.com, which introduces the concept and compares it with merge, but the best part is that it gives you two workflows how you can use rebase in a safe way:

 * Updating your feature branch with changes on the `develop` branch
 * Local Cleanup

I would definitely recommend the first one, but if you are writing good commits in the first place you shouldn't really need the second option (it's good to know about it though).

Read the article carefully: <https://www.atlassian.com/git/tutorials/merging-vs-rebasing>

?> If you want to dig deeper you can check out the [git rebase tutorial](https://www.atlassian.com/git/tutorials/rewriting-history/git-rebase) as well.

## Updating your feature branch with changes on the `develop` branch

As I said I recommend using this workflow, here is how you can set it up in terminal and any JetBrains (eg. PyCharm) product:

### git in terminal

If you are using git in terminal, it is quite easy, you just switch `git pull` to `git pull --rebase` or you could set this as the default behaviour with: `git config --global pull.rebase true`

If you have merge conflicts read the message git gives you:

```commandline
Resolve all conflicts manually, mark them as resolved with
"git add/rm <conflicted_files>", then run "git rebase --continue".
```

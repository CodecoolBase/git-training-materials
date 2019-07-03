# Writing a good Git commit message

Commit messages are important to anyone who will be reading your history. They
should be useful and readable.

Read the following article, then try the quiz below:

* [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)

It's also important for the commits to be *atomic*: a commit should do one
thing at a time. If you are making several changes, split them into separate
commits. Here is a guide:

* [Atomic Commits with Git](https://seesparkbox.com/foundry/atomic_commits_with_git)

## Quiz

Look at the following commit messages, and explain what is wrong with them. What
would be a better message?

Messages:

1. `Adding a feature to update user profile`
2. `Add parameters to the get_users function`
3. `Split the user module into user_data and user_actions, because these are two independent sets of functions`
4. `working correctly now`
5. `Obsługa połączenia z bazą danych`
6. `Add styles for login page and improve formatting of login.py`

<details>
<summary><b>Click here to see the answers.</b></summary>

1. The message doesn't use the imperative mood. This is not a big deal, but
   it's good when all messages are written in a consistent style.

   Better: `Add a feature to update user profile`

2. The message says *what* you're doing, but not *why*. What are these
   parameters for? Why did you add them?

   Better: `Support filtering by date in get_users function`

3. The commit message is too long. It might not display correctly in a terminal
   or in Github's interface.

   It's OK to have a detailed explanation of what the commit does and why, but
   you should put it in description, below the title. Remember to leave an
   empty line between title and description.

   Better:

   ```
   Split the user module into user_data and user_actions

   These are two independent sets of functions, so splitting the file
   will improve readability.
   ```

4. The message doesn't explain what is working and why. You should explain what
   you managed to fix.

   Better: `Fix the login form crashing on empty input`

5. The message has to be in English! Even if you don't have foreign developers in
   your team right now, someone could come and read the history later. And the
   commits stay forever.

   Better: `Connect to the database`

6. It looks like this commit does two different things. It would be better to
   make two separate commits.

   Better:
   * `Add styles for login page`
   * `Improve formatting of login.py`

</details>

# Objective 3: Write a Pull Request that Won't Push Others Away

As mentioned in the last objective, a `pull request (/PR)` is a formal request to make changes
to the main codebase (aka the `origin`).  There are often two parties involved in
pull requests: the contributor, and reviewer(s).

Contributors `make a PR`. However, they don't simply knock on the origin's door,
plunk down a phonebook of code, shake their tired arms and walk away.

The `contributor` solicits reviewers for their `pull request`,
and strives to make their contribution digestible via concise description,
and possibly screenshots.

Software projects often enumerate `coding standards`. The `reviewer` is responsible for
upholding these `standards`. This can be in terms of patterns, naming conventions, logic, etc.
Consistency is a prized attribute of maintainable software, and the `PR code review` is where
this can be upheld.


## Title and Describe PRs with Style

As an example, look at the following image.
It has several qualities that come together to make it slap.

This `pull request` aimed for a clear & concise `title`, and fired off bullet points
in the `description` block to hit some specifics.

Not only are these helpful for the reviewer, they make the project history (`git log`)
easier to scan.

A picture might be even better!  You can add pics to your PR Description
straight from your clipboard, like in the 2nd screenshot below ("Tempo 5.8 Chips").

**How to copy a screenshot to your clipboard**
* Windows: `win+shift+s` - crop a portion of your screen with your mouse
* Mac: `cmd+ctrl+shift+4` - crop a portion of your screen with your mouse

![img_5.png](img_5.png)

![img_7.png](img_7.png)


## Walk Through
> **Prerequisites** You'll need a strata github account to complete the walk through.

**In this walk through we're going to:**
1. Checkout an existing, never-before-merged branch
2. Make a highly detailed PR
3. Solicit a reviewer
4. Discuss our code change
5. Put on our Reviewer hat and approve the change


### Prepare a Branch to PR
Fork and clone the Git Gud repo.

1. Fork it on GitHub.com.
2. Download/clone it.
1. Run `git clone git@github.com:[yourgithubusername]/git-gud.git`
   * Not working? Try `git clone https://github.com/[yourgithubusername]/git-gud.git`
   * Still not working? Breakout room or try later
2. Run `git checkout objective-3-demo`

> For the sake of this demo, **we're going to pretend
> you created this branch, and are fully aware of the changes within it!**

### Create the PR
From GitHub.com, click xxx to make the pr.

### Write a Title and Description for the PR

Since we're only pretending you authored this branch, but are
asking you to title and describe the PR, you'll of course need
to unearth its purpose.

Scroll down to see the change.

(pic)

Now that you know what's changed, take a minute to think about
a clear but brief title for the change.  If you feel more details
would help, place those in the description block.

(pic)




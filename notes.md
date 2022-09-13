# git-gud
> This line didn't exist when the branch was created off main

Inspired by that Rust guy's tutorial, [A half Hour to Learn Rust](https://fasterthanli.me/articles/a-half-hour-to-learn-rust).

As a theme, You are a datascientist and notice there is bad data
in the list of Bee Swatter's Midwest Regional 2022 Hi Scores Dataset.
Specifically, it is missing your top score.

Never petty, simply wanting to shine a light on the situation, download
the data set, make a change, and push it back so the world can see the Truth!

Truth, after all, still does matter.

## Objective 1: Identify Core Concepts of Version Control

> Keywords are `highlighted`, and are worth understanding.

1. A `repository` is where your code is stored. It can be thought of as a folder or hard drive.
2. Copies of a repository can live anywhere: on a web server like Github.com or on your hard drive. In other words, copies are `distributed` across one or many physical locations.
3. In modern development, one of these locations is referred to as the `origin`. This is arbitrary, but is most likely the repository on github.com or bitbucket.org. Though the copy on your hard drive can also be designated as the `origin`.
4. Referring to a repository the `origin` is also just a convention.  And this means contributors to the repository agree to treat it as the master copy.
5. Copying a repository is known as `cloning`. You can refer to your copy as your `local workspace`.
6. There's another, advanced way of cloning known as `forking`, but we'll discuss that another time.
7. Having a `clone` is a great way to backup your code. If one machine dies, the code does not!
8. But there's more to your repository. You can also save every change you make.
9. Changes are segmented by `commits`.
10. Literally change one or many files in the repo.  By `committing` the changes, you create a state your can return to, should the need arise.
11. Some developers commit often. The choice is up to you. Generally commit at least once a day, just incase you spill coffee on your laptop tomorrow.
12. With a change committed, you now want to update the origin. Do this by making a `pull request`.
13. A pull request is where you ask the owner of another copy of your repository to pull your changes into their copy.  This can happen between any two clones, though typically are requested for the `origin`.

### Terminology To Master
 * `repository`
 * `origin`
 * `clone`
 * `local workspace`
 * `stage`
 * `commit` A noun, and a verb. To bookmark the state of your code.

#### Rough Draft Notes for this objective
* Should we discuss branching now or later? End by introducing it? But develop it in the next objective?

## Objective 2: Make a Significant change to Software
#### Rough Draft Notes for this objective
* Exercise: clone a repo, create a file, stage it, commit it. See the change on github.com
* explain branching. Always branch. Explain PR.
* Exercise: branch, add another file, stage it, commit it, push to origin, make a PR.
* Make a PR, find a reviewer, merge your own code
* Dive deeper into a commit: the anatomy of a nice commit message

## Objective 3: Peacefully Resolve a Conflict
#### Rough Draft Notes for this objective

## Objective 4: Restore Old Code
#### Rough Draft Notes for this objective
* discuss squashing? The beauty of helpful commit messages.
* Finding a working version through helpful log messages
* The idea of main, and tags.
* The camp that says CI/CD, don't branch--but that's for another time.
 

## General Brainstorming
 * Can I create a GitHub Action users can invoke that forces a Conflict?
 * Put each Objective into its own HTML file. Have a menu for users to click to it.
 * Host this tutorial on GitHub Pages.
 * Do the commands in a callout, like that Rust guy does.

# From Slack - put into 9-14-22 Talk
For our next git chat, is there anything in particular you'd like to go over?  RSVP if you like, and I can set up a poll if it makes sense.  Thanks!
Our Git Gud repo has 2 more objectives and Draper thought of one:
1. How to resolve a Merge Conflict
2. How to Restore a previous Commit
3. How to link a Pull Request to a Jira Ticket

Anything else that might be helpful?

Meredith Dodd
4.  How to send pull requests to others for approval and what to do when you’re approving pull requests. I think we touched on it slightly last week but it might be good to go into more depth. For instance, your pull requests come with lovely notes at the top and I don’t know how to do that!
Also maybe best practices for naming and deleting branches?

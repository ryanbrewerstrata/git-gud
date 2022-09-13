![image](https://user-images.githubusercontent.com/87713850/188872399-e949bf16-3468-4062-a870-ad6db6395332.png)

# Objective 1: Identify Core Concepts of Software Development with Git

> Core concepts are `highlighted` below.

1. A `repository` is where your code is stored. A `"repo"` can be thought of as a special folder on your machine.
2. Copies of a `repository` can live anywhere: in the cloud like Github.com or on your hard drive. In other words, copies are distributed across one or many physical locations. They are connected.
3. The original repo is referred to as the `origin`. It is owned by the project maintainers, and is the master copy.
4. Copying a repository is known as `cloning`. You can refer to your copy as your `local workspace`.
5. A `clone` is complete copy of your repo and its history. It's a great backup. If one machine dies, the code does not!
6. Changes to your code are contained in `branches`.
7. Branches are considered short-lived, and should be deleted after the code is merged into the `main` branch.
8. Save your code changes by first `staging` the files, then making a `commit` to your local `repo`.
9. Commits are annotated with a description of your change.
10. It's not wrong or right to commit often or infrequently. Just know coffee can be spilt on your laptop at any time.
11. A codebase's history of commits can be reviewed, and any commit can be restored.
12. With a change committed to your local repo, you now want to `push` your branch to the origin.
13. Once your `branch` is on the `origin`, others can see it and `pull` it into their local workspace.
14. When ready, your code changes can be `merged` into the `main` branch.
15. Typically, a `repo's` `main` branch is protected, and cannot be changed without an approved `pull request`.
16. A `pull request` is a formal request to the repo maintainers to review and approve your changes.
17. Once approved, your branch can be `merged` into `main`, and deleted.
18. Your changes will be seen by users once the `main` branch is deployed in the next release.


## Terminology from this Objective
 * `repository (/repo)` Where software is stored, maintained, and developed.
 * `origin` The original repo, owned by the project maintainers 
 * `clone` A copy of a repo and its entire history
 * `local workspace` Your local copy of a repo. Your edits won't affect the repo until they have been staged and committed.
 * `branch` A named space for your changes and commits, typically aligned with a feature or bug fix.
 * `main` A special branch. The trunk. The origin's main branch is what gets deployed, and is often protected from unapproved changes. Most branches stem off main.
 * `stage` File changes can be selected or deselected for saving in a commit. This is called staging.
 * `commit` Saves your staged file changes to the repo. Has a description of the change. Once committed, your changes within the commit can be seen by others and restored.
 * `push` Your local branch (with its changes committed) will be pushed to the origin
 * `pull` Your local repo can pull branches (and commits) from the origin to get updates
 * `pull request (/PR)` Asking the maintainers of the origin to review and merge your branch's changes into main
 * `merge` After a pull request is approved, it is merged into the main branch

## Tips & Tricks
 * Your code changes can be linked to JIRA tickets!  You do this by creating a branch with the Jira ticket id.  Eg,
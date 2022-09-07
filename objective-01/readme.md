# Objective 1: Identify Core Concepts of Version Control

> Core concepts are `highlighted` below.

1. A `repository` is where your code is stored. A `"repo"` can be thought of as a special folder on your machine.
2. Copies of a `repository` can live anywhere: in the cloud like Github.com or on your hard drive. In other words, copies are distributed across one or many physical locations. They are connected.
3. In modern development, one of these connected locations is referred to as the `origin`. This designation is arbitrary, but is most likely a repository in the cloud.
4. Referring to a `repository` as the `origin` is also just a convention.  It means maintainers agree it is the master copy.
5. Copying a repository is known as `cloning`. You can refer to your copy as your `local workspace`.
6. A `clone` is complete copy of your code and its history. It's a great backup. If one machine dies, the code does not!
7. Changes to your code are contained in `branches`.
8. Branches are considered short-lived, and should be deleted after the code is merged into the `main` branch.
9. Save your code changes by first `staging` the files, then making a `commit` to your local `repo`.
10. Commits are annotated with a description of your change.
11. It's not wrong or right to commit often or infrequently. Just know coffee can be spilt on your laptop at any time.
12. A codebase's history of commits can be reviewed, and any commit can be restored.
13. With a change committed to your local repo, you now want to `push` your branch to the origin.
14. Once your branch lives at the origin, others can see it and `pull` into their local workspace, if they wanted.
15. When ready, your code changes can be merged into the main branch.
16. Typically, repo's main branch is protected, and cannot be changed without an approved `pull request`.
17. A pull request is a formal request to the repo maintainers to review and approve your changes.
18. Once approved, your branch can be `merged` into main, and deleted.


## Terminology from this Objective
 * `repository (/repo)` Where software is stored, maintained, and developed.
 * `origin` The original repo, owned by the project maintainers 
 * `clone` A copy of a repo and its entire history
 * `local workspace` Your local copy of a repo. Your edits won't affect the repo until they have been staged and committed.
 * `branch` A named space for your changes and commits, typically aligned with a feature or bug fix
 * `main` A special branch. The origin's main branch is what gets deployed, and is often protected from unapproved changes.
 * `stage` File changes can be selected or deselected for saving in a commit. This is called staging.
 * `commit` Saves your staged file changes to the repo. Has a description of the change. Once committed, your changes within the commit can be seen by others and restored.
 * `push` Your local branch (with its changes committed) will be pushed to the origin
 * `pull` Your local repo can pull branches (and commits) from the origin to get updates
 * `pull request (/PR)` Asking the maintainers of the origin to review and merge your branch's changes into main
 * `merge` After a pull request is approved, it is merged into the main branch
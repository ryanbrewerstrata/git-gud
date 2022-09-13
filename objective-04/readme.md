# Objective 4: Peacefully Resolve a Conflict

> **Completion of Objective 3 is required.** This objective starts where that one ends.

## Noticing a conflict

(Pic of conflict in github)

The red text indicates a problem, and that you cannot merge your code.

What you're seeing is a `merge conflict`. But what is this?

Git requires that everyone agrees on the past.
It does this by remembering how each branch begins and ends,
and comparing beginnings.

That is to say if your branch has a line that began in main as "x", and when you go to merge it
main now says that line is "y", you get a `merge conflict`.
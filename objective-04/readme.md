# Objective 4: Peacefully Resolve a Conflict on GitHub

> **Completion of Objective 3 is required.** This objective starts where that one ends.

## Noticing a conflict

(Pic of conflict in GitHub)

The red text indicates a problem, and that you cannot merge your code.

What you're seeing is a `merge conflict`. But what is this?

Git requires that everyone agrees on the past.
It does this by tracking how each branch begins and ends,
and compares beginnings.

That is to say if your branch has a line that began in main as "x",
and when you attempt to merge it was changed to "y",
you'll get a `merge conflict`.

![img_1.png](img_1.png)


## Resolving a conflict in GitHub

1. Click the Resolve Conflict button
2. For this demo, we're going to agree our line is the right line, and what is in Main can be overwritten. Delete the
arrows, divider, and old line so that the file looks like your initial change.

(pic of resolve conflict button)

(pic of the conflict in the editor)


## More about our Resolution

Many conflicts aren't as trivial as this one. In some cases you'll consult with the author of the conflicting
code and decide together how best to move forward.  Additionally, there are more advanced tools than the one
demo'd today on GitHub.  Many IDEs, like PyCharm and VSCode have more tools to help you understand and fix a conflict.
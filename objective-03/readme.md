# Objective 3: Create a Highly Detailed Pull Request

As mentioned in the last objective, a `pull request (/PR)` is a formal request to make changes
to the main codebase (aka the `origin`).  There are often two parties involved in
pull requests: the contributor, and reviewer(s).

Contributors `make a PR`. However, they don't simply knock on the origin's door,
plunk down a phonebook of code, and skip off on their merry way.

The `contributor` solicits reviewers for their `pull request`,
and strives to make their contribution digestible via concise description,
and possibly screenshots.

Software projects often enumerate `coding standards`. The `reviewer` is responsible for
upholding these `standards`. This can be in terms of patterns, naming conventions, logic, etc.
Consistency is a prized attribute of maintainable software, and the `PR code review` is where
to keep it.

**In this walkthrough, we're going to:**
1. Checkout an existing, never-before-merged branch
2. Make a highly detailed PR
3. Solicit a reviewer
4. Discuss our code change
5. Put on our Reviewer hat and approve the change


## Prepare a Branch to PR

If you haven't already, clone the git gud repo so you have a copy on your machine.

1. Run `git clone git@github.com:ryanbrewerstrata/git-gud.git`
   * Not working? Try `git clone https://github.com/ryanbrewerstrata/git-gud.git`
   * Still not working? Breakout room.
2. Run `git checkout origin/objective-3-demo` 


#### Rough Draft Notes for this objective
* Responsibilities & Etiquette on contribution. For the Maker and Reviewer.
* How to write nice PRs
  * When you make the PR you can enter a title, and description
  * Strive for clarity + brevity
  * Imperative tone
  * Use markdown!
    * Go over the Basics of markdown + link to cheat sheet
    * You can practice MarkDown in Slack!
  * Adding nice screenshots gives context to your peers
    * Harrison showed last week if you have a screenshot on your clipboard (windows + shift + s)(ctrl + shift + command + 4) you can paste it in!
    * PyCharm does the same thing! (Requires the Markdown plugin.)
  * If more clarity is needed, you can leave comments on lines of code.
  * Broader conversations can also be held on the main PR page.
  * Once approved, merge your own code. Might have to wait for a build process to finish.
  * After merging to main, github can automatically delete the branch on the origin. You can delete your local branch if you like.  Remember to switch back to main and pull.
* How to add a Reviewer
  * Top right of your pr. Can add a reviewer at any time. Most projects of ours require 1 approver.
* How to be a reviewer
  * Look in email, or on GitHub.com
  * Ask clarifying questions
  * You can comment on particular line of code, or more broadly
  * Come from a place of verified trust. It's ok to rubber stamp if your team is experienced.
  * For long-lived and large projects Consistency is highly valued. Ensure code changes uphold existing team standards. Come to an agreement with your team.
  * How to Approve
  * If the code is edited, a new approval may be required
* Linking GitHub to Jira (does it happen by branch name or pr or both?)
  * Note: Compare (BEN Jira project) cannot create a branch on github for you--it has old configuration and if you click the Jira ticket's Create Branch button it tries to make one on BitBucket, which is deprecated.
  * If you make a branch locally and push it to the origin, it takes a few min but Jira will pick it up.
    * Requires ticket id, eg, BEN-4030
      * 12:15 I created branch and pushed to origin.
      * 12:42, not seen on jira. 
      * 12:50 it was there! 30+ minutes to show up on jira?
  * If you make a PR w/o ticket id, it will still show up in jira. Took roughly an hour. 1:45pm. Might be that Jira only scans once an hour!
  * What about if you make a branch w/o ticket info but put ticket info in PR title?
    * Result: 


![img_3.png](img_3.png)

![img_1.png](img_1.png)
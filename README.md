# Guidelines

## Information regarding this repository :eyes:

Although most of the important guidelines are listed here, there may be things that were missed!  If you feel confused about something and think it should be addressed here,
please submit an issue.  You can learn how to do this [here](https://help.github.com/articles/creating-an-issue/).


## Using Git and Github :octocat:

* A handy cheatsheet of git commands can be seen [here](https://services.github.com/on-demand/downloads/github-git-cheat-sheet/).

* A handy cheatsheet of git terminology can be seen [here](https://help.github.com/articles/github-glossary/).  This may be useful to familiarize yourself with before reading these guidelines.

* If you are new to Git or Github, you should read through [this](https://guides.github.com/introduction/git-handbook/) to familiarize yourself with basic terms and concepts.
We are willing to help you learn, but taking the initiative to read through this is important too. It's okay to not completely understand everything here at first, but getting
familiar will help us help you!


## Making Commits :pencil2:

Commits should have descriptive messages that state not WHAT you changed, but rather WHY you changed it.  

Remember: we generally know how to read your code, but we might not know why you did it!
If you feel that your code is unclear as to WHAT you changed as well, *only then* is it necessary to state the "what" in the commit message.
The only other time the "what" is appropriate is if the "why" is self-evident, such as adding a comment or fixing a typo.

Examples of a good commit message:
```bash
$ git commit -m "Added the ability to assign judges to projects"
$ git commit -m "Make Source.indexOf(ByteString) significantly faster"
```

An example of a bad commit message:
```bash
$ git commit -m "Added a function"
$ git commit -m "Changes"
$ git commit -m "Added main.py file"
```

Any commit that has a poor commit message will **NOT** be merged until it is fixed.  To learn how to change your commit message, see [here](https://help.github.com/articles/changing-a-commit-message/).

Please make sure that all files you are committing fit the commit message.  If something feels like it doesn't belong, it is most likely best to put it in a new separate commit.


## Making Pull Requests :mailbox_with_mail:

* To learn how to make a pull request (PR), see [here](https://help.github.com/articles/creating-a-pull-request/).

* **NEVER EVER EVER** push directly to the master branch. In fact, we block you from being able to do this! Please make a PR first from a fork or another branch.

* **EVERY** pull request made on must have at least one reviewer that approves it.
If the code contribution is significant (a new feature, large commits, etc.) there must be at least two approving reviewers.
If you feel your contribution is just too significant, it is okay to request a group review at a team meeting, or a meeting with another teammate!
You can explain your changes to the group, and your group will discuss them in the meeting.

* Be sure to name your pull request well, and follow similar rules to the commit message rules above.  Describe the purpose of the PR.
Additionally, add more of a description if the feature is significant or if the changes are extensive (lots of new or changed code, etc).
Sometimes, particularly for front end changes, screenshots can be very helpful!

* For all front end changes, please ensure that you have tested your code on both desktop and mobile.  If your PR does not work for both, it will likely
not be merged.

* For all changes, please ensure to the best of your ability that the project runs as expected, and that the code that you added works.  We do not want
anybody submitting broken code in PRs!  Take pride in your code and make sure that it is everything it is intended to be! :smiley:

TL;DR **TEST YOUR CODE**


## Proper Documentation :books:

All repositories should include a descriptive README file (preferably written in markdown) that includes, at a minimum, the following:

* A description of the project
	* What does it do?
	* What languages and frameworks are used?
	* What features does it have?
	* Where is it hosted? (if at all)

* How to run the project
	* What commands need to be run?
	* What needs to be installed?

* Contribution guidelines
	* What do you want to make sure that everybody knows when they contribute?
	* How should code be formatted?

Additionally, all code should be well documented within each file.  Make sure that the people that read your code understand what it's doing.
But be careful not to add comments where the code is already self-evident.  We don't want to crowd the code with too many comments!

Examples of good comments:
```python
# Process the CSV file that contains submissions data from Devpost
```

Examples of unnecessary comments:
```python
foo = 0 # Initialize to zero
```

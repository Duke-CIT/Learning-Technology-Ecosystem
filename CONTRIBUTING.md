# Contributing

Admittedly, we are using `origin` + `upstream` mostly because @profmikegreene hasn't figured out how to get the Duke-CIT github organization repo to work on his machine with gitbook. Thanks to @sakaiproject for this great documentation.

## Workflow

 * ***local*** = A copy of the repo on your workstation (this is where everyone typically does work)
* ***origin*** = Your personal copy of the repo on GitHub (you `clone` this repository on your workstation to make the ***local*** copy for everyday work)
* ***upstream*** = Main GitHub repo (everyone forks this project into their GitHub account to make the ***origin***)

To work on and contribute to Learning Technology Ecosystem:

1. [Set up Git, create a GitHub account, and set your name and e-mail address correctly as Git global variables on your local workstation](https://help.github.com/articles/set-up-git/)

2. `install` Gitbook via NodeJS (v4.0.0 and above is recommended)

	`npm install gitbook-cli -g`

3. [Fork](https://help.github.com/articles/fork-a-repo/) the [central repository](https://github.com/Duke-CIT/Learning-Technology-Ecosystem) to your own GitHub account

4. `Clone` your ***origin*** repository onto your local workstation (this example uses HTTPS as the transport mechanism):

  `git clone https://github.com/GITHUBACCOUNTNAME/Learning-Technology-Ecosystem`
 
5. Add a `remote` to receive updates from the ***upstream*** repository:

  `git remote add upstream https://github.com/Duke-CIT/Learning-Technology-Ecosystem`

6. Update your ***local*** repository frequently to stay up to date:

  `git checkout master` (switch to ***local*** `master` branch)
  
  `git pull upstream master` (`pull` in any ***upstream*** changes)
  
  `git push origin master` (`push` the changes up to the ***origin***)



## Working on bugs and features

#### Never work in your ***local*** `master` branch.

This branch should always be the same as what is in  ***upstream*** `master` and if you make commits into your ***local*** `master`, and those commits are not accepted into the upstream repository `master`, you will forever be maintaining them yourself, which can get very complicated. To make life easier for yourself, **use a branch for everything**.

### General workflow

To fix a bug or add a feature, the general Git workflow is:

1. Create a ***local*** branch using Github Issue reference for the branch name:

  `git checkout -b 4-patch-name`


2. Do work

3. Preview work with `gitbook serve` and view at [http://localhost:4000](http://localhost:4000)

4. Add changed or new files:

  `git add .`

5. Make your ***local*** commit:

  `git commit -m "#4 Add some documentation about contributing"`

6. Share branch back to ***origin***:

  `git push origin 4-patch-name`

7. [Create a pull request (PR)](https://help.github.com/articles/creating-a-pull-request/) using GitHub from the branch against the ***upstream*** `master` for review by others

### Respond to a pull request (PR) by updating proposed changes

You will often receive friendly advice to improve or fix the changes you proposed in a p. To update your changes and maintain the existing PR, you should:
  
1. Change to your ***local*** branch:

  `git checkout 4-patch-name`

2. Make changes and/or improvements in response to PR comments

3. Add changed or new files:

  `git add -u`

4. Update existing commit (this updates the previous commit rather than making a new one):

  `git commit --amend -C HEAD`

5. Share your new ***local*** changes back to the ***origin*** branch and the original PR (by force is required for amending commits. You should only ever push by force into your own repo):

  `git push -f origin 4-patch-name`

6. Make a comment on the existing PR to alert reviewers to your changes

[Edit on Gitbook](https://www.gitbook.com/book/profmikegreene/the-learning-technology-ecosystem/edit#/edit/master/{{file.path}})

[Edit on Github](https://github.com/Duke-CIT/Learning-Technology-Ecosystem/edit/


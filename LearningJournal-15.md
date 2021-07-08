# LearningJournal-15

Class 8/jul/2021

# Git & GitHub  


- Start from an up-to-date _main_ branch
  - `git checkout main`
  - `git pull origin main`
  - Create a new feature branch with `git checkout -b <branchname>`
- Do work on your feature branch and **add**, **commit**, and **push**
  - `git add <file>`
  - `git commit -m <useful message>`
  - `git push origin <feature_branch_name>`
- On GitHub...
  - Create a Pull Request (PR) for that branch on GitHub
  - Have someone else review the code in the PR and merge it

## Time for a Merge Party!

**WHEN A PULL REQUEST FROM SOMEONE ELSE'S \<FEATURE BRANCH> IS MERGED TO main, EVERYONE MUST DO THESE STEPS**

- commit changes to your _feature branch_
  - `git add <file>`
  - `git commit -m <useful message>`
- update your local _main_ branch
  - `git checkout main`
  - `git pull origin main`
- update your _feature branch_ with changes in _main_
  - `git checkout <feature_branch_name>`
  - `git merge main`
- handle merge conflicts _if there are any_
  - Check all of your project files for the markers that indicate merge conflicts (in other words, the `>>>>>>>>>` and `HEAD` stuff that has mysteriously appeared in your code)
  - Edit the code to remove the redundancies causing the merge conflict, and eliminate the markers
  - `git add <affected-files>`
  - `git commit -m "merged main"`
  - `git push origin <feature_branch_name>`

## Project Organization

Here is some more information about GH Organizations....

Create an organization by clicking on the plus sign in the top right corner of GitHub. Then, create your repository(ies) within the organization.
All team members should be added as collaborators on the organization.

Within the repository, click on the "Project" tab and then click the button to "Create a project".
This will allow you to create a project board associated with the repository. Make several columns with meaningful names,
such as "To-Do", "In progress", "Under review", and "Completed".

Populate your project with issues. Each issue should be a small item, typically linked to a feature task.
As you work on an issue, assign it to yourself and move it into the "In progress" column.
This will provide an easy way for everyone on the team to see the progress of each issue and know who is working on a particular issue.

_Why:_
> Issues are userful for managing small features that an individual or pair can reasonably tackle in a short period of time.
>  The project board creates a clear visual of the team's current tasks and the current project status.

When using GitHub issues, there is the added benefit of being able to close an issue through a commit message or a comment on a pull request (PR).
For example, a commit message or comment can say "Closes #42" and the issue will automatically be closed when the pull request is merged.
Github recognizes the following keywords to close an issue: `close`, `closes`, `closed`, `fixes`, and `fixed`.

You are welcome to use other project management tools besides GitHub Projects, but your code base must be on GitHub.


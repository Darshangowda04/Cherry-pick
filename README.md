7 0+

Ans)

To create a lightweight Git tag named v1.0 for a commit in your local repository, use the following 

command:

git tag v1.0

This command creates a lightweight tag for the current commit.

And to show the tag on git hub use

git push origin v1.0
_______________________________
8 Write the command to cherry-pick a range of commits from "source-branch" to the current

branch.

Ans)>Create one branch called feature branch with some commits

git checkout main

you will get Switched to branch 'main'

use git log feature-branch

To show all the logs of the feature branch as shown below

commit 1777dfc0045ca4824c6388276fc71fb322e83751 (feature-branch)

Author: w3schools-test <test@w3schools.com>

Date: Tue Nov 19 20:23:11 2024 +0530

Add change in feature branch

Cherry pick commnd syntax like shown below

git cherry-pick commit hash


ex:

Use git cherry-pick 1777dfc0045ca4824c6388276fc71fb322e83751(commit hash) to move this 

commit to main branch
_______________________________
9)Given a commit ID, how would you use Git to view the details of that specific commit,

including the author, date, and commit message

ans)

To view the details of a specific commit, including the author, date, and commit message, use the 

following Git command:

git show <commit-id>

This command will display:

• The commit ID

• Author name and email

• Commit date

• Commit message

• A diff of the changes introduced by the commit
_______________________________
Program 10

Analyzing and Changing Git History

Write the command to list all commits made by the author "John Doe" between

"2023-01-01" and "2023-12-31."

git log --author=<Name>--since=<Date>/--after=<Date>

git log

====

Example :use this below syntax for the above command

git log --author="John Doe" --since="2023-01-01" –until="2023-12-31"
_______________________________
Program 11

Analyzing and Changing Git History

Write the command to display the last five commits in the repository's history

Example : git log -5

For exmple to give last 2 commits use git log 2

output is

=============

commit 5acbf338128b5b8b3ff2a196d93c837c8b3c71b3 (HEAD -> main, origin/main, origin/HEAD)

Author: AI and ML student <atmestudent.edu.in>

Date: Tue Dec 3 12:48:27 2024 +0530

 Initial commit

commit 7efae202aa270c7ed54870c52bcffcd80e07a468

Author: AI and ML student <atmestudent.edu.in>

Date: Wed Nov 27 12:42:40 2024 +0530

 empty
_______________________________
Program 12

Analyzing and Changing Git History

Write the command to undo the changes introduced by the commit with the ID

"abc123".

Syntax uis

git revert commit-id

 for the above case use git tevert abc123

For Practical Example usage see below

git revert 5acbf338128b5b8b3ff2a196d93c837c8b3c71b3

git push origin main




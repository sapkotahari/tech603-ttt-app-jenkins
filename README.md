Tic Tac Toe app code to be used with Jenkins for CI/CD pipeline

Set up job 1 and build trigger to test the webhook in GitHub.

Created a dev branch, then line added to test job1 triggers with push to dev branch

created job2-merge to merge dev to main.

forgot to add post-build actions in job1, which meant  jobs 1 and 2 weren't linked. As a result only job1 ran after git push to dev.
But now they are linked.

Added git merge dev in execute shell in job2-merge

added git merge origin/dev in execute shell in job2-merge

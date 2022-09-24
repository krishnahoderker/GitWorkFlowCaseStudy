# GitWorkFlowCaseStudy
GitWorkFlowCaseStudy

Branch Structure"
Master
The master branch stores the official release history 

Develop :
Develop branch serves as an integration branch for features.

Feature :
Each new feature should reside in its own branch, which can be pushed to the central repository for backup/collaboration. But, instead of branching off of master, feature branches use develop as their parent branch. 
When a feature is complete, it gets merged back into develop. 
Features should never interact directly with master.


Git Workflow:
Every new collaborater will create a new branch from develop branch and work on their respective feature branch.
Once feature is complete, concerned collaborater will push their changes to their respective remote feature branch.
They will also be responsible to raise pull request to review and merge their changes to develop branch for the code cutoff.
Please ensure to add your team lead as reviewer for the change.

Team lead will review and if pull request changes looks good then Team lead will push those changes to develop, If not, then concerned collaborator has to work on addiional changes suggested as per review comments and make changes in the same branch.
Mark pull request conversations as resolved if applicable.

Team lead will build develop branch on code cutoff and build collective changes on the test server for QA.

If QA logs issues, then respective collaborator will make those changes in the same feature branch and raise a new pull request for the fixes done with destination branch as develop until all the concerned issues are resolved.

Upon QA team sign off, changes will be merged to master branch for the release.

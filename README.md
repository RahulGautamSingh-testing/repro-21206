## Debug Log

```log
DEBUG: syncBranchState() 
DEBUG: syncBranchState(): update baseBranch name 
DEBUG: branch.isUpToDate(): using cached result "true"    // this needs to change
...
DEBUG: Checking if PR has been edited 
DEBUG: branch.isModified(): using git to calculate 
DEBUG: branch.isModified() = false 
DEBUG: Found existing branch PR 
DEBUG: PR has been edited, PrNo:1   // incorrectly assumes that targetBranch was changed by user when actually user changed baseBranch in renovate-config
DEBUG: Ensuring comment to indicate that rebasing is not possible 
DEBUG: Getting comments for #1 
DEBUG: Found 0 comments 
DEBUG: Ensuring comment "Edited/Blocked Notification" in #1 
 INFO: Comment added 
       "issueNo": 1,
       "topic": "Edited/Blocked Notification"
```

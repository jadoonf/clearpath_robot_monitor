# clearpath_robot_monitor
Add repos with file paths to be monitored to repos.json. The action will create a job for each path in each repo. An issue is created for each commit which contains one of the files mentioned since the date in its tracking file.  The tracking file will just take the form .sync/{owner}/{repo}/{path}. When adding a new repo/file path the action will create the tracking file with the current time.

## Issues with poll-github-repo/action:
* Only monitors default branch
* Action takes a single file only

## Features which we eould add to poll-github-repo/action
* Automatically create sync file
* Create issues in another project

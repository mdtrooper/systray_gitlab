# Systray Gitlab

A simple systray applet for gitlab in python to get notifications and quick view of the boring tasks sended by your jobmates.

## Notes

The [gitlab API Rest v4](https://docs.gitlab.com/ee/api/rest/) has a lot bugs, for example you can get a issue (by iid) from endpoint `/issues?iids[]=number_issue` (it returns a empty list) but if you call endpoint `projects/<id_project>/isssues?iids[]=number_issue`, yes the buggy api returns the issue.
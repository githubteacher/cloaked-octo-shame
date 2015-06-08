

Settings
git config --global core.autcrlf true
git config --global core.editor
…
user.name
user.email

git config
system – per computer
global – per logged in user
local – per repository


Recommend to create the repository remotely (and then clone from URL)

Commit up to 50 characters. Use extended description. Describe the motivation. The new line gets you to the extended description

Branching is cheap

Push only from my fb to fb remote
git config --global push.default simple

cache credentials (in seconds):
git config --global credential.helper "cache --timeout=30000"
(can generate "personal access token" and use it as password after applying this command)

Merge
Fast forward? Depends…
You can use "command line" link to get tips for manual merge commands
The green button uses no fast forward

creates the remote branch
git push –u …
doesn't affect history..

Aliases
git config –global alias.<some_alias> "<some_command_without_git>"
git config --global alias.lga "log --oneline --decorate --all --graph"
'!git fetch && git merge'
Why !?
Why single quote

File name are case insensitive because Git ignores case by default, by configuring:
core.ignrecase=true

checkboxes
in comment, issues etc.
- [] some desc 1
- [] some desc 2

GitHub Keyboard Shortcuts
Shift+?

Revert
The revert button creates a new branch, commit the opposite merge changes and creates a new pull request
Revert command:
git revert
if there was a manual merge:
git revert –m <parent number>
in most cases you want to use parent number 1 (before the manual merge)


CONTRIBUTING.md – in root directory will be used for some instructions



GitHub Company dos and don'ts
-	Deploy feature branch to production! After verifying master is in
-	Fork? Not @GitHub
o	Overhead (hard to keep the fork up-to-date).
o	GitHub encourage to give write access to all and merge to master

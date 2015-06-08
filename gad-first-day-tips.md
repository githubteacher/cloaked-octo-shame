# First day tips

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


GitHub
Deploy feature branch to production! After verifying master is in
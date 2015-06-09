### Tips

#### Show Current Git Branch in Prompt
There are many variants of this. Here's one approach, for `Bash` shells. Create a file called `git_branch.sh` defining this function:
```bash
#!/bin/bash

# get Git branch name
git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
```

Make sure that file's in your `PATH`, and use it in your `~/.bashrc`:
```bash
# show current git branch in prompt
export PS1="\w\[\033[36m\]\$(git_branch.sh) \[\033[00m\] > "
```

# git mv
Git doesn't track file movement. But it has a mv command as a convenience function:
`git mv old_file new_file`

It translates to:
`git rm old_file`
`git add new_file`

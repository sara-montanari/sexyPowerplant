# This is a header
### This is a smaller header

nano is a text editor
.md is a Markdown file

when we created this file it was untracked (= not committed to git)
then we added it to git wiht git add and now it is committed

after editing this file it appears as modified and untracked and the old version remains committed as new file in git status
if we are happy wiht the edits we can added to git again, the modified file disappear from the untracked list,
the new file that is committed is the one with modifications

### add then commit
wiht commit -m you can add a message to yor file in git

### use checkout to change order of versions of committed files
i.e. git checkout HEAD~1 file --> the last version is now the current verison
git checkout HEAD file --> now back to the current version as current version

### compare versions
git diff HEAD HEAD~3 file
this will compare the current version wiht the version 3 modifications ago

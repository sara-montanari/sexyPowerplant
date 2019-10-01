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
i.e.
git checkout HEAD~1 file --> change to the previous version that was committed
git checkout HEAD file --> now back to the current version ((committed)

Cannot do if versions are not committed, they will be lost wiht checkout

After checkout to another version, commit to save it as the latest committed version

### list filt to ignore, i.e. not to add to the repo
nano .gitignore
list files to ignore here, can use wildcards
usually you want to ignore data files, such as csv or fastq

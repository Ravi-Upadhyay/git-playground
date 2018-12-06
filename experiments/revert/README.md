# GIT Revert Experiment

## Objective

How `git revert` is being used. Is this able to revert any older commit in the history (not immediate one). Can i revert reverted commit again. 

I had a typical problem where in one commit I deleted several files. After few months I realised that older approach was good one. I wanted to get those files back. I went one commit down from where I deleted the files, From there I created a new branch and manually done the changes which I done on later commits. I found that as I merge new branch which has all deleted files as well as code which i have written after that into master whole files lost again. (3 way merge). 

So the way is to revert that particular commit.

## Process Followed

1. First we created `txt-file-1.txt` and commited `937598f First Commit for revert experiment`.
2. Then we created `txt-file-2.txt` and commited `6060350 Second commit for revert experiment`.
3. Then we reverted commit we created in step-1 that is `937598f First Commit for revert experiment`.
    1. Use `git revert 937598f`.
    2. Only file which we created on first commit has been lost `txt-file-1.txt`.
    3. New commit formed at the top. `9726b12 Revert "First Commit for revert experiment"`
4. Then we reverted the commit `9726b12 Revert "First Commit for revert experiment"` to ensure that whether reverted commit can be revert back so we can get the file back.
    1. Use `git revert 9726b12`
    2. File from first commit `txt-file-1.txt` came back.

## Conclusion


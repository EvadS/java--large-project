

## Installing Git LFS
to go to the git-lfs [website](https://git-lfs.com/) and install the files


### new repository
```
git lfs install
```

git add .gitattributes





### exists repository
```
git reflog expire --expire-unreachable=now --all
git gc --prune=now
```
#### Code explanation
```
git reflog expire --expire-unreachable=now --all
```
This command removes entries from the reflog that are unreachable. The reflog records when references
 were updated in your repository. By using --expire-unreachable=now,
 it immediately expires all unreachable reflog entries. The --all flag applies this to all references.

```
git gc --prune=now
```
 This command runs garbage collection to clean up unnecessary files and optimize the repository. The --prune=now option removes objects that are unreachable from any reference, immediately cleaning up space.
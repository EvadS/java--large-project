
# How to use Git-lfs ( Large File Storage )

## Installing Git LFS
to go to the git-lfs [website](https://git-lfs.com/) and install the files

## init git repo
```bash
 git init
```
```bash
    git add .
```
```bash
git  commit -m 'initial commit'
```

### setup git lfs
```bash
git lfs install
```

### select the file types that you want Git-lfs to manage using the command
```bash
git lfs track “*.dic”
```
### add large file to .gitattributes
```bash
 git add .gitattributes .\src\main\resources\static\ukrainian.dic
```

### commit push
```bash
    git commit -m "ukrainian dic"
    git push origin master
````
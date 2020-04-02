# bash-lib-dependency-manager
Bash lib dependency manager to retrieve bash files from Github repo

**Usage:**
Create a file _dependencies.list_ and add dependencies on separate lines with following format:
```
repoOwner,repoName,releaseTag,fileName
```
Example:
```
aldrinbaroi,bash-lib-logging,0.1,bash-lib-logging,lib
```

In the bash script, add the following line:
```
source dependency-manager
```
The bash files will be downloaded _once_ and saved under "lib" folder. To force redownload, delete the downloaded file from the "lib" folder.


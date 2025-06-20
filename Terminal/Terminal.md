**Basics**
```bash
clear         # clear screen
man ls        # open mannual for each command
ls -a         # flags
```
**Navigation**
```bash
ls            # list files (show files)
ls -a         # list with hidden files and folders
pwd           # print working directory (where I am?)

# change directory
cd folderName              # change directory
cd Downloads/LocalSend     # multiple steps
cd 'My Folder'             # for more than a word

# Paths
cd Downloads/LocalSend        # relative path
cd /User/abino/Files1/Files2  # absolute path (can be access from anywhere)
    # '/' for root directory
    # '~' for home directory

# back
cd ~              # back to home directory
cd ..             # one-step back
cd ../..          # two-step back

# create files and folders
mkdir 'File Name'  # Used to create folders
touch index.html   # Used to create files (also for modifing date and time)

# deleting files and folders
rm index.html app.js style.css   # removes files
rmdir emptyFolder                # removes empty folders
rm -rf                           # removes any folder (recurssive force)
```
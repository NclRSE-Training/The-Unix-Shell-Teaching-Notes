## Background
GUI
CLI

## The Shell
- command line
- shell
- dos box
- terminal
- $ - bash shell
- % - korn, c shell

# Unix Shell
wget https://swcarpentry.github.io/shell-novice/data/shell-lesson-data.zip
unzip shell-lesson-data.zip

# Episode 2 Navigating Files and Directories

## Home Directory Variation
![Filesystem](https://newcastlerse-training.github.io/carpentries-unix-exercises/fig/filesystem.svg)

## Slashes
![File System 2](https://newcastlerse-training.github.io/carpentries-unix-exercises/fig/home-directories.svg)


## Commands
```bash
ls
pwd
ls -F
clear
ls --help
man ls
ls -j
```
[Exercises](episode2_ex.md)

```bash
ls -F Desktop
ls -F Desktop/shell-lesson-data
cd Desktop
cd shell-lesson-data
cd data
pwd
cd shell-lesson-data
cd ..
pwd
cd Desktop/shell-lesson-data/data
pwd
cd /Users/nelle/Desktop/shell-lesson-data
pwd
ls -F
cd ~
cd -
cd ..
cd ~/Desktop/shell-lesson-data
cd creatures
cd -

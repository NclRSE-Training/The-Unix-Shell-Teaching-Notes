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

## Exploring Other Directives
```bash
ls -F Desktop
ls -F Desktop/shell-lesson-data
cd Desktop
cd shell-lesson-data
cd data
pwd
ls -F
cd shell-lesson-data
ERROR
cd ..
pwd
cd Desktop/shell-lesson-data/data
pwd
ls -F -a
```

## Other Hidden Files

    In addition to the hidden directories .. and ., you may also see a file called .bash_profile. This file usually contains shell configuration settings. You may also see other files and directories beginning with .. These are usually files and directories that are used to configure different programs on your computer. The prefix . is used to prevent these configuration files from cluttering the terminal when a standard ls command is used.

These three commands are the basic commands for navigating the filesystem on your computer: pwd, ls, and cd. Let’s explore some variations on those commands. What happens if you type cd on its own, without giving a directory?

```bash
cd
pwd
cd Desktop/shell-lesson-data/data

pwd
cd /Users/nelle/Desktop/shell-lesson-data
pwd
ls -F
```
## Shortcuts
```
cd ~
cd -
cd ..


cd ~/Desktop/shell-lesson-data
cd creatures
cd -
```
[Exercises](episode2_ex2.md)

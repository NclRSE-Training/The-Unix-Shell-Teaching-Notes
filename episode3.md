# Episode 3: Working With Files and Directories

```bash
pwd
ls -f
```

## Create a directory
```bash
mkdir thesis
ls -F
ls -F thesis
mkdir -p project/data project/results
ls -RF
```
The ```-R``` option to the ls command will list all nested subdirectories within a directory. Let’s use ls ```-FR``` to recursively list the new directory hierarchy we just created in the project directory:
```bash
ls -FR project
```
## Two ways of doing the same thing

You can also use File Explorer 

## Good names for files and directories

    Complicated names of files and directories can make your life painful when working on the command line. Here we provide a few useful tips for the names of your files and directories.

1. Don’t use spaces: Spaces can make a name more meaningful, but since spaces are used to separate arguments on the command line it is better to avoid them in names of files and directories. You can use - or _ instead (e.g. north-pacific-gyre/ rather than north pacific gyre/). To test this out, try typing mkdir north pacific gyreand see what directory (or directories!) are made when you check with ls -F.

1. Don’t begin the name with - (dash): Commands treat names starting with - as options.

1. Stick with letters, numbers, . (period or ‘full stop’), - (dash) and _ (underscore): Many other characters have special meanings on the command line. We will learn about some of these during this lesson. There are special characters that can cause your command to not work as expected and can even result in data loss.

If you need to refer to names of files or directories that have spaces or other special characters, you should surround the name in quotes (```""```).

## Create a text file
```bash
cd thesis
nano draft.txt
```

## Which Editor
### Nano
![Controls](https://newcastlerse-training.github.io/carpentries-unix-exercises/fig/controls.PNG)

```bash
ls
```
[Exercise](expisode3_ex1.md)

### What's In a Name?
Extensions: 
1. .txt
2. .pdf
3. .cfg
4. .png
5. whale.mp3

## Moving files and Directories

```bash
cd ~/Desktop/shell-lesson-data/
mv thesis/draft.txt thesis/quotes.txt
ls thesis
mv thesis/quotes.txt .
ls thesis
ls thesis/quotes.txt - ERROR
ls quotes
```

[Exercises](expisode3_ex2.md)

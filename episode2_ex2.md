## 2.3 Absolute vs Relative Paths
Starting from `/Users/amanda/data`, which of the following commands could Amanda use to navigate to her home directory, which is `/Users/amanda`?

1. `cd .`
2. `cd /`
3. `cd /home/amanda`
4. `cd ../..`
5. `cd ~`
6. `cd home`
7. `cd ~/data/..`
8. `cd`
9. `cd ..`


<details>
<summary>Solution
</summary>


1. No: `.` stands for the current directory.
<br>
2. No: `/` stands for the root directory.
<br>
3. No: Amanda's home directory is `/Users/amanda`.
<br>
4. No: this goes up two levels, i.e. ends in `/Users`.
<br>
<strong>5. Yes: `~` stands for the user's home directory, in this case `/Users/amanda`.</strong>
<br>
6. No: this would navigate into a directory `home` in the current directory if it exists.
<br>
<strong>7. Yes: unnecessarily complicated, but correct.</strong>
<br>
<strong>8. Yes: shortcut to go back to the user's home directory.</strong>
<br>
<strong>9. Yes: goes up one level.</strong>
</details>

## 2.4 Relative Path Resolution
If `pwd` displays `/Users/thing`,
 what will `ls -F ../backup` display?
1.  `../backup: No such file or directory`
2.  `2012-12-01 2013-01-08 2013-01-27`
3.  `2012-12-01/ 2013-01-08/ 2013-01-27/`
4.  `original/ pnas_final/ pnas_sub/`

![File System for Challenge Questions](fig/filesystem-challenge.svg)


<details>
<summary>Solution  
</summary>
1. No: there *is* a directory `backup` in `/Users`.  
<br>
2. No: this is the content of `Users/thing/backup`, but with `..` we asked for one level further up.  
<br>
3. No: see previous explanation.  
<br>
<strong>4. Yes: `../backup/` refers to `/Users/backup/`.</strong>
</details>

## 2.5 `ls` Reading Comprehension

If `pwd` displays `/Users/backup`,
and `-r` tells `ls` to display things in reverse order,
what command(s) will result in the following output:

~~~
pnas_sub/ pnas_final/ original/
~~~

![File System for Challenge Questions](fig/filesystem-challenge.svg)

1.  `ls pwd`

2.  `ls -r -F`

3.  `ls -r -F /Users/backup`

<details>
<summary>Solution
</summary>
1. No: `pwd` is not the name of a directory.
<br>
<strong>2. Yes: `ls` without directory argument lists files and directories in the current directory.</strong>
<br>
<strong>3. Yes: uses the absolute path explicitly.</strong>
</details>

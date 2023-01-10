## 2.5 `ls` Reading Comprehension

If `pwd` displays `/Users/backup`,
and `-r` tells `ls` to display things in reverse order,
what command(s) will result in the following output:

~~~
pnas_sub/ pnas_final/ original/
~~~

![File System for Challenge Questions](https://newcastlerse-training.github.io/carpentries-unix-exercises/fig/filesystem-challenge.svg)

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

[Episode 3 Exercise 1](episode3_ex1.md)

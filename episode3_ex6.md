## 3.6 Copy with Multiple Filenames

 For this exercise, you can test the commands in the `shell-lesson-data/data` directory.

 In the example below, what does `cp` do when given several filenames and a directory name?

 ~~~
 $ mkdir backup
 $ cp amino-acids.txt animals.txt backup/
 ~~~


 In the example below, what does `cp` do when given three or more file names?

 ~~~
 $ ls -F
 ~~~

 ~~~
 amino-acids.txt  animals.txt  backup/  elements/  morse.txt  pdb/  planets.txt  salmon.txt  sunspot.txt
 ~~~

 ~~~
 $ cp amino-acids.txt animals.txt morse.txt
 ~~~


<details>
<summary>Solution
</summary>

 If given more than one file name followed by a directory name (i.e. the destination directory must
 be the last argument), <code>cp</code> copies the files to the named directory.

 If given three file names, <code>cp</code> throws an error, because it is expecting a directory
 name as the last argument.
</details>

[Episode 3 Exercise 7](episode3_ex7.md)

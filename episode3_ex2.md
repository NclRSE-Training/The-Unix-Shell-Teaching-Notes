## 3.2 Moving Files to a new folder

Jamie realizes that she put the files `sucrose.dat` and `maltose.dat` into the wrong folder. 
The files should have been placed in the `raw` folder. She runs these commands to explore the file system.

~~~
$ ls -F
analyzed/ raw/

$ ls -F analyzed
fructose.dat glucose.dat maltose.dat sucrose.dat

$ cd analyzed
 ~~~


Fill in the blanks to move these files to the `raw/` folder to correct her mistake

 ~~~
$ mv sucrose.dat maltose.dat ____/____
~~~

<details>
<summary>Solution
</summary>
  
<code>
$ mv sucrose.dat maltose.dat ../raw
 </code>
  
 Recall that <code>..</code> refers to the parent directory (i.e. one above the current directory) and that <code>.</code> refers to the current directory.
</details>

[Episode 3 exercise 3](episode3_ex3.md)

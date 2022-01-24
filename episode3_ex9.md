## 3.9 Organizing Directories and Files

Jamie is working on a project and she sees that her files aren’t very well organized:

```bash
$ ls -F
```
```output
analyzed/  fructose.dat    raw/   sucrose.dat
```

The fructose.dat and sucrose.dat files contain output from her data analysis. What command(s) covered in this lesson does she need to run so that the commands below will produce the output shown?

```bash
$ ls -F
```
```output
analyzed/   raw/
```
```bash
$ ls analyzed
```
```output
fructose.dat    sucrose.dat
```

<details>
  <summary>
Solution
  </summary>

<pre>
  mv *.dat analyzed
  </pre>

  Jamie needs to move her files <code>fructose.dat</code> and <code>sucrose.dat</code> to the <code>analyzed</code> directory. The shell will expand *.dat to match all .dat files in the current directory. The <code>mv</code> command then moves the list of .dat files to the ‘analyzed’ directory.



</details>

[Episode 3 Exercise 10](episode3_ex10.md)

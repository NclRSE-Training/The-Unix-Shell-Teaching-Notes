## 5.2 Variables in Loops

This exercise refers to the ```shell-lesson-data/molecules``` directory. ```ls``` gives the following output:

```output
cubane.pdb  ethane.pdb  methane.pdb  octane.pdb  pentane.pdb  propane.pdb
```

What is the output of the following code?

```bash
$ for datafile in *.pdb
> do
>     ls *.pdb
> done
```

Now, what is the output of the following code?

```bash
$ for datafile in *.pdb
> do
>     ls $datafile
> done
```

Why do these two loops give different outputs?

<details>
  <summary>
Solution
  </summary>

The first code block gives the same output on each iteration through the loop. Bash expands the wildcard <code>*.pdb</code> within the loop body (as well as before the loop starts) to match all files ending in <code>.pdb</code> and then lists them using <code>ls</code>. The expanded loop would look like this:

  
  <pre>
$ for datafile in cubane.pdb  ethane.pdb  methane.pdb  octane.pdb  pentane.pdb  propane.pdb
> do
>     ls cubane.pdb  ethane.pdb  methane.pdb  octane.pdb  pentane.pdb  propane.pdb
> done
</pre>
  
  <pre>
cubane.pdb  ethane.pdb  methane.pdb  octane.pdb  pentane.pdb  propane.pdb
cubane.pdb  ethane.pdb  methane.pdb  octane.pdb  pentane.pdb  propane.pdb
cubane.pdb  ethane.pdb  methane.pdb  octane.pdb  pentane.pdb  propane.pdb
cubane.pdb  ethane.pdb  methane.pdb  octane.pdb  pentane.pdb  propane.pdb
cubane.pdb  ethane.pdb  methane.pdb  octane.pdb  pentane.pdb  propane.pdb
cubane.pdb  ethane.pdb  methane.pdb  octane.pdb  pentane.pdb  propane.pdb
</pre>

The second code block lists a different file on each loop iteration. The value of the <code>datafile</code> variable is evaluated using <code>$datafile</code>, and then listed using <code>ls</code>.

<pre>
cubane.pdb
ethane.pdb
methane.pdb
octane.pdb
pentane.pdb
propane.pdb
</pre>

</details>

[Episode 5 Exercise 3](episode5_ex3.md)

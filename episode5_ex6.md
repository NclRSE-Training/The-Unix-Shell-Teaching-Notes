## 5.6 Doing a Dry Run

A loop is a way to do many things at once — or to make many mistakes at once if it does the wrong thing. One way to check what a loop would do is to echo the commands it would run instead of actually running them.

Suppose we want to preview the commands the following loop will execute without actually running those commands:

```bash
$ for datafile in *.pdb
> do
>     cat $datafile >> all.pdb
> done
```

What is the difference between the two loops below, and which one would we want to run?

```bash
# Version 1
$ for datafile in *.pdb
> do
>     echo cat $datafile >> all.pdb
> done
```

```bash
# Version 2
$ for datafile in *.pdb
> do
>     echo "cat $datafile >> all.pdb"
> done
```

<details>
  <summary>
Solution
  </summary>

The second version is the one we want to run. This prints to screen everything enclosed in the quote marks, expanding the loop variable name because we have prefixed it with a dollar sign. It also does not modify nor create the file <code>all.pdb</code>, as the <code>>></code> is treated literally as part of a string rather than as a redirection instruction.
<br>
The first version appends the output from the command <code>echo cat $datafile</code> to the file, <code>all.pdb</code>. This file will just contain the list; <code>cat cubane.pdb</code>, <code>cat ethane.pdb</code>, <code>cat methane</code>.pdb etc.
<br>
Try both versions for yourself to see the output! Be sure to open the <code>all.pdb</code> file to view its contents.
</details>

[Episode 5 Exercise 7](episode5_ex7.md)

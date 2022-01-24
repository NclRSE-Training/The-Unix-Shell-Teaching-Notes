## 4.3 Appending Data

We have already met the ```head``` command, which prints lines from the start of a file. ```tail``` is similar, but prints lines from the end of a file instead.

Consider the file ```shell-lesson-data/data/animals.txt```. After these commands, select the answer that corresponds to the file ```animals-subset.txt```:

```bash
$ head -n 3 animals.txt > animals-subset.txt
$ tail -n 2 animals.txt >> animals-subset.txt
```

1. The first three lines of ```animals.txt```
1. The last two lines of ```animals.txt```
1. The first three lines and the last two lines of ```animals.txt```
1. The second and third lines of ```animals.txt```

<details>
  <summary>
Solution
  </summary>

  Option 3 is correct. For option 1 to be correct we would only run the <code>head</code> command. For option 2 to be correct we would only run the <code>tail</code> command. For option 4 to be correct we would have to pipe the output of <code>head</code> into <code>tail -n 2</code> by doing <code>head -n 3 animals.txt | tail -n 2 > animals-subset.txt</code>

</details>
[Episode 4 Exercise 3.md](episode4_ex3.md)

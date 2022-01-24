## 4.7 Which Pipe?

The file ```animals.txt``` contains 8 lines of data formatted as follows:

```output
2012-11-05,deer
2012-11-05,rabbit
2012-11-05,raccoon
2012-11-06,rabbit
...
```

The ```uniq``` command has a ```-c``` option which gives a count of the number of times a line occurs in its input. Assuming your current directory is ```shell-lesson-data/data/```, what command would you use to produce a table that shows the total count of each type of animal in the file?

1. ```sort animals.txt | uniq -c```
1. ```sort -t, -k2,2 animals.txt | uniq -c```
1. ```cut -d, -f 2 animals.txt | uniq -c```
1. ```cut -d, -f 2 animals.txt | sort | uniq -c```
1. ```cut -d, -f 2 animals.txt | sort | uniq -c | wc -l```

<details>
  <summary>
Solution
  </summary>

Option 4. is the correct answer. If you have difficulty understanding why, try running the commands, or sub-sections of the pipelines (make sure you are in the <code>shell-lesson-data/data</code> directory).

</details>

[Episode 4 Exercise 8](episode4_ex8.md)

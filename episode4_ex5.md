## 3.5 Pipe Reading Comprehension

A file called ```animals.txt``` (in the ```shell-lesson-data/data``` folder) contains the following data:

```bash
2012-11-05,deer
2012-11-05,rabbit
2012-11-05,raccoon
2012-11-06,rabbit
2012-11-06,deer
2012-11-06,fox
2012-11-07,rabbit
2012-11-07,bear
```

What text passes through each of the pipes and the final redirect in the pipeline below?

```bash
$ cat animals.txt | head -n 5 | tail -n 3 | sort -r > final.txt
```

Hint: build the pipeline up one command at a time to test your understanding

<details>
  <summary>
Solution
  </summary>

  The <code>head</code> command extracts the first 5 lines from <code>animals.txt</code>. Then, the last 3 lines are extracted from the previous 5 by using the <code>tail</code> command. With the <code>sort -r</code> command those 3 lines are sorted in reverse order and finally, the output is redirected to a file <code>final.txt</code>. The content of this file can be checked by executing <code>cat final.txt</code>. The file should contain the following lines:

2012-11-06,rabbit
2012-11-06,deer
2012-11-05,raccoon

</details>

[Episode 4 Exercise 6](episode4_ex6.md)

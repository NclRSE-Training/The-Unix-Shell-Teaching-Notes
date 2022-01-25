## 6.4 Find the Longest File With a Given Extension

Write a shell script called ```longest.sh``` that takes the name of a directory and a filename extension as its arguments, and prints out the name of the file with the most lines in that directory with that extension. For example:

```bash
$ bash longest.sh shell-lesson-data/data/pdb pdb
```

would print the name of the ```.pdb``` file in ```shell-lesson-data/data/pdb``` that has the most lines.

Feel free to test your script on another directory e.g.

```bash
$ bash longest.sh shell-lesson-data/writing/data txt
```

<details>
  <summary>
Solution
  </summary>
  <pre><code># Shell script which takes two arguments:
#    1. a directory name
#    2. a file extension
# and prints the name of the file in that directory
# with the most lines which matches the file extension.

wc -l $1/*.$2 | sort -n | tail -n 2 | head -n 1</code></pre>

  The first part of the pipeline, <code>wc -l $1/*.$2 | sort -n</code>, counts the lines in each file and sorts them numerically (largest last). When there’s more than one file, <code>wc</code> also outputs a final summary line, giving the total number of lines across all files. We use <code>tail -n 2 | head -n 1</code> to throw away this last line.

  With <code>wc -l $1/*.$2 | sort -n | tail -n 1</code> we’ll see the final summary line: we can build our pipeline up in pieces to be sure we understand the output.
</details>

[Episode 6 Exercise 5](episode6_ex5.md)

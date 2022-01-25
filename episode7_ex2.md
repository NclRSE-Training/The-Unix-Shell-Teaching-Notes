## 7.2 Tracking a Species

Leah has several hundred data files saved in one directory, each of which is formatted like this:

```
2013-11-05,deer,5
2013-11-05,rabbit,22
2013-11-05,raccoon,7
2013-11-06,rabbit,19
2013-11-06,deer,2
```

She wants to write a shell script that takes a species as the first command-line argument and a directory as the second argument. The script should return one file called ```species.txt``` containing a list of dates and the number of that species seen on each date. For example using the data shown above, ```rabbit.txt``` would contain:

```
2013-11-05,22
2013-11-06,19
```

Put these commands and pipes in the right order to achieve this:

```bash
cut -d : -f 2
>
|
grep -w $1 -r $2
|
$1.txt
cut -d , -f 1,3
```

Hint: use ```man grep``` to look for how to grep text recursively in a directory and ```man cut``` to select more than one field in a line.

An example of such a file is provided in ```shell-lesson-data/data/animal-counts/animals.txt```

<details>
  <summary>
Solution
  </summary>

  <pre><code>grep -w $1 -r $2 | cut -d : -f 2 | cut -d , -f 1,3 > $1.txt</code></pre>

Actually, you can swap the order of the two cut commands and it still works. At the command line, try changing the order of the cut commands, and have a look at the output from each step to see why this is the case.
<br>
You would call the script above like this:

  <pre><code>$ bash count-species.sh bear .</code></pre>
</details>

[Episode 7 Exercise 3](episode7_ex3.md)

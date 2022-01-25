## 6.6 Debugging Scripts

Suppose you have saved the following script in a file called ```do-errors.sh``` in Nelle’s ```north-pacific-gyre/2012-07-03``` directory:

```bash
# Calculate stats for data files.
for datafile in "$@"
do
echo $datfile
bash goostats.sh $datafile stats-$datafile
done
```

When you run it:

```bash
$ bash do-errors.sh NENE*A.txt NENE*B.txt
```

the output is blank. To figure out why, re-run the script using the ```-x``` option:

```bash
$ bash -x do-errors.sh NENE*A.txt NENE*B.txt
```

What is the output showing you? Which line is responsible for the error?

<details>
  <summary>
Solution
  </summary>

  The <code>-x</code> option causes <code>bash</code> to run in debug mode. This prints out each command as it is run, which will help you to locate errors. In this example, we can see that <code>echo</code> isn’t printing anything. We have made a typo in the loop variable name, and the variable <code>datfile</code> doesn’t exist, hence returning an empty string.
</details>

[Episode 7 Exercise 1](episode7_ex1.md)

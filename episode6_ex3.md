## 6.3 Variables in Shell Scripts

In the molecules directory, imagine you have a shell script called script.sh containing the following commands:

```bash
head -n $2 $1
tail -n $3 $1
```

While you are in the molecules directory, you type the following command:

```bash
$ bash script.sh '*.pdb' 1 1
```

Which of the following outputs would you expect to see?

1. All of the lines between the first and the last lines of each file ending in ```.pdb``` in the ```molecules``` directory
2. The first and the last line of each file ending in ```.pdb``` in the ```molecules``` directory
3. The first and the last line of each file in the ```molecules``` directory
4. An error because of the quotes around ```*.pdb```

<details>
  <summary>
Solution
  </summary>

The correct answer is 2.

The special variables $1, $2 and $3 represent the command line arguments given to the script, such that the commands run are:

  <pre><code>$ head -n 1 cubane.pdb ethane.pdb octane.pdb pentane.pdb propane.pdb
$ tail -n 1 cubane.pdb ethane.pdb octane.pdb pentane.pdb propane.pdb</code></pre>

  The shell does not expand <code>'*.pdb'</code> because it is enclosed by quote marks. As such, the first argument to the script is <code>'*.pdb'</code> which gets expanded within the script by <code>head</code> and <code>tail</code>.
</details>

[Episode 6 Exercise 4](episode6_ex4.md)

## 6.5 Script Reading Comprehension

For this question, consider the ```shell-lesson-data/molecules``` directory once again. This contains a number of ```.pdb``` files in addition to any other files you may have created. Explain what each of the following three scripts would do when run as ```bash script1.sh *.pdb```, ```bash script2.sh *.pdb```, and ```bash script3.sh *.pdb``` respectively.

```bash
# Script 1
echo *.*
```

```bash
# Script 2
for filename in $1 $2 $3
do
cat $filename
done
```

```bash
# Script 3
echo $@.pdb
```

<details>
  <summary>
Solutions
  </summary>

  In each case, the shell expands the wildcard in <code>*.pdb</code> before passing the resulting list of file names as arguments to the script.
<br>
Script 1 would print out a list of all files containing a dot in their name. The arguments passed to the script are not actually used anywhere in the script.
<br>
Script 2 would print the contents of the first 3 files with a <code>.pdb</code> file extension. <code>$1</code>, <code>$2</code>, and <code>$3</code> refer to the first, second, and third argument respectively.
<br>
Script 3 would print all the arguments to the script (i.e. all the <code>.pdb</code> files), followed by <code>.pdb</code>. <code>$@</code> refers to all the arguments given to a shell script.
  <pre><code>cubane.pdb ethane.pdb methane.pdb octane.pdb pentane.pdb propane.pdb.pdb</code></pre>
</details>

[Episode 6 Exercise 6](episode6_ex6.md)

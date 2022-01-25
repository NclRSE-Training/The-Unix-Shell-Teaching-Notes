
List Unique Species

Leah has several hundred data files, each of which is formatted like this:

```
2013-11-05,deer,5
2013-11-05,rabbit,22
2013-11-05,raccoon,7
2013-11-06,rabbit,19
2013-11-06,deer,2
2013-11-06,fox,1
2013-11-07,rabbit,18
2013-11-07,bear,1
```

An example of this type of file is given in ```shell-lesson-data/data/animal-counts/animals.txt```.

We can use the command ```cut -d , -f 2 animals.txt | sort | uniq``` to produce the unique species in ```animals.txt```. In order to avoid having to type out this series of commands every time, a scientist may choose to write a shell script instead.

Write a shell script called ```species.sh``` that takes any number of filenames as command-line arguments, and uses a variation of the above command to print a list of the unique species appearing in each of those files separately.

<details>
  <summary>
Solution
  </summary>
  <pre><code># Script to find unique species in csv files where species is the second data field
# This script accepts any number of file names as command line arguments
<br>
# Loop over all files
for file in $@
do
    echo "Unique species in $file:"
    # Extract species names
    cut -d , -f 2 $file | sort | uniq
done</code></pre>
</details>

[Episode 6 Exercise 2](episode6_ex2.md)

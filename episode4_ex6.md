## 4.6 Pipe Construction

For the file ```animals.txt``` from the previous exercise, consider the following command:

```bash
$ cut -d , -f 2 animals.txt
```

The ```cut``` command is used to remove or ‘cut out’ certain sections of each line in the file, and ```cut``` expects the lines to be separated into columns by a ```Tab``` character. A character used in this way is a called a **delimiter**. In the example above we use the ```-d``` option to specify the comma as our delimiter character. We have also used the ```-f``` option to specify that we want to extract the second field (column). This gives the following output:

```output
deer
rabbit
raccoon
rabbit
deer
fox
rabbit
bear
```

The ```uniq``` command filters out adjacent matching lines in a file. How could you extend this pipeline (using ```uniq``` and another command) to find out what animals the file contains (without any duplicates in their names)?

<details>
  <summary>
Solution
  </summary>

  <code>
$ cut -d , -f 2 animals.txt | sort | uniq
  </code>
  
  </details>
  
  [Episode 4 Exercise 7](episode4_ex7.md)


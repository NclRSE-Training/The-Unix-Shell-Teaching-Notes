## Using rm Safely

What happens when we execute ```rm -i thesis_backup/quotations.txt```? Why would we want this protection when using ```rm```?

<details>
  <summary>
Solution
  </summary>

<pre>
  rm: remove regular file 'thesis_backup/quotations.txt'? y
  </pre>

  The <code>-i</code> option will prompt before (every) removal (use <code>Y</code> to confirm deletion or <code>N</code> to keep the file). The Unix shell doesn’t have a trash bin, so all the files removed will disappear forever. By using the <code>-i</code> option, we have the chance to check that we are deleting only the files that we want to remove.
</detail>

[Episode 3 Exercise 6](episode3_ex6.md)

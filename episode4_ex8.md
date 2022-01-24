## 4.8 Removing Unneeded Files

Suppose you want to delete your processed data files, and only keep your raw files and processing script to save storage. The raw files end in ```.dat``` and the processed files end in ```.txt```. Which of the following would remove all the processed data files, and only the processed data files?

1. ```rm ?.txt```
1. ```rm *.txt```
1. ```rm * .txt```
1. ```rm *.*```

<details>
  <summary>
Solution
  </summary>

  <ol>
    <li>This would remove <code>.txt</code> files with one-character names</li>
    <li>This is correct answer</li>
    <li>The shell would expand <code>*</code> to match everything in the current directory, so the command would try to remove all matched files and an additional file called <code>.txt</code></li>
    <li>The shell would expand <code>*.*</code> to match all files with any extension, so this command would delete all files</li>
  </ol>

</details>

[Episode 5 Exercise 1](episode5_ex1.md)

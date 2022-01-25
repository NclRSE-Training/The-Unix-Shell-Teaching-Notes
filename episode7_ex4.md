## 7.4 Matching and Subtracting

The ```-v``` option to ```grep``` inverts pattern matching, so that only lines which do not match the pattern are printed. Given that, which of the following commands will find all files in ```/data``` whose names end in ```s.txt``` but whose names also do not contain the string ```net```? (For example, ```animals.txt``` or ```amino-acids.txt``` but not ```planets.txt```.) Once you have thought about your answer, you can test the commands in the ```shell-lesson-data``` directory.

1. ```find data -name "*s.txt" | grep -v net```
2. ```find data -name *s.txt | grep -v net```
3. ```grep -v "net" $(find data -name "*s.txt")```
4. None of the above.

<details>
  <summary>
Solution
  </summary>

The correct answer is 1. Putting the match expression in quotes prevents the shell expanding it, so it gets passed to the <code>find</code> command.
<br>
  Option 2 is incorrect because the shell expands <code>*s.txt</code> instead of passing the wildcard expression to <code>find</code>.
<br>
Option 3 is incorrect because it searches the contents of the files for lines which do not match ‘net’, rather than searching the file names.
</details>

[Episode 7 Exercise 5](episode7_ex5.md)

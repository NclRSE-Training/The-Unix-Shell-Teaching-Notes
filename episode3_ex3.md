## 3.3 Renaming Files
 Suppose you created a text file called `statstics.txt`

 After creating and saving this file you realize you misspelled the filename! You want to
 correct the mistake, which of the following commands could you use to do so?

 1. `cp statstics.txt statistics.txt`
 2. `mv statstics.txt statistics.txt`
 3. `mv statstics.txt .`
 4. `cp statstics.txt .`

<details>
<summary>Solution
</summary>
 1. No.  While this would create a file with the correct name, the incorrectly named file still exists in the directory
 and would need to be deleted.
 <br>
 <strong>2. Yes</strong>
 <br>
 3. No, the period(.) indicates where to move the file, but does not provide a new file name; identical file names
 cannot be created.
 <br>
 4. No, the period(.) indicates where to copy the file, but does not provide a new file name; identical file names
 cannot be created.
</details>

## 3.4 Moving and Copying

What is the output of the closing `ls` command in the sequence shown below?

 ~~~
 $ pwd
 ~~~

 ~~~
 /Users/jamie/data
 ~~~

 ~~~
 $ ls
 ~~~

 ~~~
 proteins.dat
 ~~~

 ~~~
 $ mkdir recombined
 $ mv proteins.dat recombined/
 $ cp recombined/proteins.dat ../proteins-saved.dat
 $ ls
~~~



 1.   `proteins-saved.dat recombined`
 2.   `recombined`
 3.   `proteins.dat recombined`
 4.   `proteins-saved.dat`

<details>
<summary>Solution
</summary>
 2. 
 <br>
Starting in the `/Users/jamie/data` directory
<br>
  $ mkdir recombined ----> create new folder
  <br>
  $ mv proteins.dat recombined/ -----> move proteins.dat to the new folder
  <br>
  $ cp recombined/proteins.dat ../proteins-saved.dat -----> copies this file to the parent directory of our current location
</details>

[Return](episode3.md)

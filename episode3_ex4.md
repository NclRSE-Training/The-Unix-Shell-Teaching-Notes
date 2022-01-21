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

[Episode 3 Exercise 5](episode3_ex5.md)

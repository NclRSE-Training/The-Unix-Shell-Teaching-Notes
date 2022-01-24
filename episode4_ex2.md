## 4.2 What Does >> Mean?

We have seen the use of ```>```, but there is a similar operator ```>>``` which works slightly differently. We’ll learn about the differences between these two operators by printing some strings. We can use the ```echo``` command to print strings e.g.

```bash
$ echo The echo command prints text
```
```output
The echo command prints text
```

Now test the commands below to reveal the difference between the two operators:

```bash
$ echo hello > testfile01.txt
```

and:

```bash
$ echo hello >> testfile02.txt
```

Hint: Try executing each command twice in a row and then examining the output files.

<details>
  <summary>
Solution
  </summary>

In the first example with ```>```, the string ‘hello’ is written to ```testfile01.txt```, but the file gets overwritten each time we run the command.

We see from the second example that the ```>>``` operator also writes ‘hello’ to a file (in this ```casetestfile02.txt```), but appends the string to the file if it already exists (i.e. when we run it for the second time).

</details>

[Episode 4 Exercise 3](episode4_ex3.md)

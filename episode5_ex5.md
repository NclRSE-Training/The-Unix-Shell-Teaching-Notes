## 5.5 Saving to a File in a Loop - Part Two

Also in the ```shell-lesson-data/molecules``` directory, what would be the output of the following loop?

```bash
> for datafile in *.pdb
> do
>     cat $datafile >> all.pdb
> done
```

1. All of the text from ```cubane.pdb```, ```ethane.pdb```, ```methane.pdb```, ```octane.pdb```, and ```pentane.pdb``` would be concatenated and saved to a file called ```all.pdb```.
2. The text from ```ethane.pdb``` will be saved to a file called ```all.pdb```.
3. All of the text from ```cubane.pdb```, ```ethane.pdb```, ```methane.pdb```, ```octane.pdb```, ```pentane.pdb``` and ```propane.pdb``` would be concatenated and saved to a file called ```all.pdb```.
4. All of the text from ```cubane.pdb```, ```ethane.pdb```, ```methane.pdb```, ```octane.pdb```, ```pentane.pdb``` and ```propane.pdb``` would be printed to the screen and saved to a file called ```all.pdb```.

<details>
  <summary>
Solution
  </summary>
  3 is the correct answer. <code>>></code> appends to a file, rather than overwriting it with the redirected output from a command. Given the output from the cat command has been redirected, nothing is printed to the screen.
</details>

[Episode 5 Exercise 6](episode5_ex6.md)

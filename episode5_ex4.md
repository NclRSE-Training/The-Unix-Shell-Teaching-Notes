## 5.4 Saving to a File in a Loop - Part One

In the ```shell-lesson-data/molecules``` directory, what is the effect of this loop?

```bash
> for alkanes in *.pdb
> do
>    echo $alkanes
>    cat $alkanes > alkanes.pdb
> done
```

1. Prints ```cubane.pdb```, ```ethane.pdb```, ```methane.pdb```, ```octane.pdb```, ```pentane.pdb``` and ```propane.pdb```, and the text from ```propane.pdb``` will be saved to a file called ```alkanes.pdb```.
2. Prints ```cubane.pdb```, ```ethane.pdb```, and ```methane.pdb```, and the text from all three files would be concatenated and saved to a file called ```alkanes.pdb```.
3. Prints ```cubane.pdb```, ```ethane.pdb```, ```methane.pdb```, ```octane.pdb```, and ```pentane.pdb```, and the text from ```propane.pdb``` will be saved to a file called ```alkanes.pdb```.
4. None of the above.

<details>
  <summary>
Solution
  </summary>
The text from each file in turn gets written to the <code>alkanes.pdb</code> file. However, the file gets overwritten on each loop iteration, so the final content of <code>alkanes.pdb</code> is the text from the <code>propane.pdb</code> file.
</details>

[Episode 5 Exercise 5](episode5_ex5.md)

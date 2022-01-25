## 5.3 Limiting Sets of Files

What would be the output of running the following loop in the ```shell-lesson-data/molecules``` directory?

```bash
$ for filename in c*
> do
>     ls $filename
> done
```

No files are listed.
All files are listed.
Only ```cubane.pdb```, ```octane.pdb``` and ```pentane.pdb``` are listed.
Only ```cubane.pdb``` is listed.

<details>
  <summary>
Solution
  </summary>
4 is the correct answer. ```*``` matches zero or more characters, so any file name starting with the letter c, followed by zero or more other characters will be matched.
</details>
  
How would the output differ from using this command instead?

```bash
$ for filename in *c*
> do
>     ls $filename
> done
```

The same files would be listed.
All the files are listed this time.
No files are listed this time.
The files ```cubane.pdb``` and ```octane.pdb``` will be listed.
Only the file ```octane.pdb``` will be listed.

<details>
  <summary>
Solution
  </summary>

4 is the correct answer. ```*``` matches zero or more characters, so a file name with zero or more characters before a letter c and zero or more characters after the letter c will be matched.
</details>

[Episode 5 Exercise 4](episode5_ex4.md)

## 3.1 Creating Files a Different Way

We have seen how to create text files using the nano editor. Now, try the following command:

```python
$ touch my_file.txt
```

1. What did the touch command do? When you look at your current directory using the GUI file explorer, does the file show up?
1. Use ```ls -l``` to inspect the files. How large is ```my_file.txt```?
1. When might you want to create a file this way?


<details>
  <summary>
Solution
  </summary>

  <ol>
    <li>The touch command generates a new file called <code>my_file.txt</code> in your current directory. You can observe this newly generated file by typing <code>ls</code> at the command line prompt. <code>my_file.txt</code> can also be viewed in your GUI file explorer.</li>
    <li>When you inspect the file with <code>ls -l</code>, note that the size of my_file.txt is 0 bytes. In other words, it contains no data. If you open <code>my_file.txt</code> using your text editor it is blank.</li>
<li>Some programs do not generate output files themselves, but instead require that empty files have already been generated. When the program is run, it searches for an existing file to populate with its output. The touch command allows you to efficiently generate a blank text file to be used by such programs.</li>
  </ol>

</details>

[Episode 3 Exercise 2](episode3_ex2.md)

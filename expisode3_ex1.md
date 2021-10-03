# Creating Files a Different Way

We have seen how to create text files using the nano editor. Now, try the following command:

~~~bash
$ touch my_file.txt
~~~

1. What did the touch command do? When you look at your current directory using the GUI file explorer, does the file show up?
1. Use ls -l to inspect the files. How large is my_file.txt?
1. When might you want to create a file this way?

<details>
<summary>Solution
</summary>
  
1. The ```touch``` command generates a new file called ```my_file.txt``` in your current directory.  You can observe this newly generated file by typing `ls` at the command line prompt.  ```my_file.txt``` can also be viewed in your GUI file explorer.
  
2. When you inspect the file with ```ls -l```, note that the size of ```my_file.txt``` is 0 bytes.  In other words, it contains no data. If you open ```my_file.txt``` using your text editor it is blank.
  
3. Some programs do not generate output files themselves, but instead require that empty files have already been generated. When the program is run, it searches for an existing file to populate with its output.  The touch command allows you to efficiently generate a blank text file to be used by such programs.
</details>

[Return](expisode3.md)

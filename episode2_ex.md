## 2.1 Exploring More `ls` Flags

What does the command `ls` do when used
with the `-l` option? 

What about if you use both the `-l` and the `-h` option?

<details>
<summary>Solution
</summary>
`-l` - long listing format, showing not only the file/directory names but also additional information such as the file size and the time of its last modification. Some of its output is about properties that we do not cover in this lesson (such as file permissions and ownership), but the rest should be useful nevertheless.   
 
`-h` + `-l`  - makes file size ‘Human readable’, i.e. `5.3K` instead of `5369`.
</details>




## 2.2 Listing in Reverse Chronological Order
By default ls lists the contents of a directory in alphabetical order by name. The command `ls -t` lists items by time of last change instead of alphabetically. The command `ls -r` lists the contents of a directory in reverse order. What happens when you combine the `-t` and `-r` flags? Hint: You may need to use the `-l` flag to see the last changed dates.

<details>
<summary>Solution

</summary>
`-t` - most recently changed file first.    

`-rt` - most recently changed file last.  

This can be very useful for finding your most recent edits or checking to see if a new output file was written.
</details>



[Return](episode2.md)

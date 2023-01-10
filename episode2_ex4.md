## 2.4 Relative Path Resolution
If `pwd` displays `/Users/thing`,
 what will `ls -F ../backup` display?
1.  `../backup: No such file or directory`
2.  `2012-12-01 2013-01-08 2013-01-27`
3.  `2012-12-01/ 2013-01-08/ 2013-01-27/`
4.  `original/ pnas_final/ pnas_sub/`

![File System for Challenge Questions](https://newcastlerse-training.github.io/carpentries-unix-exercises/fig/filesystem-challenge.svg)


<details>
<summary>Solution  
</summary>
1. No: there *is* a directory `backup` in `/Users`.  
<br>
2. No: this is the content of `Users/thing/backup`, but with `..` we asked for one level further up.  
<br>
3. No: see previous explanation.  
<br>
<strong>4. Yes: `../backup/` refers to `/Users/backup/`.</strong>
</details>

[Episode 2 Exercise 5](episode2_ex5.md)

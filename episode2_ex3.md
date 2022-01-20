## 2.3 Absolute vs Relative Paths
Starting from `/Users/amanda/data`, which of the following commands could Amanda use to navigate to her home directory, which is `/Users/amanda`?

1. `cd .`
2. `cd /`
3. `cd /home/amanda`
4. `cd ../..`
5. `cd ~`
6. `cd home`
7. `cd ~/data/..`
8. `cd`
9. `cd ..`


<details>
<summary>Solution
</summary>


1. No: `.` stands for the current directory.
<br>
2. No: `/` stands for the root directory.
<br>
3. No: Amanda's home directory is `/Users/amanda`.
<br>
4. No: this goes up two levels, i.e. ends in `/Users`.
<br>
<strong>5. Yes: `~` stands for the user's home directory, in this case `/Users/amanda`.</strong>
<br>
6. No: this would navigate into a directory `home` in the current directory if it exists.
<br>
<strong>7. Yes: unnecessarily complicated, but correct.</strong>
<br>
<strong>8. Yes: shortcut to go back to the user's home directory.</strong>
<br>
<strong>9. Yes: goes up one level.</strong>
</details>

[Episode 2 Exercise 4](episode2_ex4.md)

## 4.4 Piping Commands Together

In our current directory, we want to find the 3 files which have the least number of lines. Which command listed below would work?

1. wc -l * > sort -n > head -n 3
1. wc -l * | sort -n | head -n 1-3
1. wc -l * | head -n 3 | sort -n
1. wc -l * | sort -n | head -n 3

<details>
  <summary>
Solution
  </summary>

  Option 4 is the solution. The pipe character <code>|</code> is used to connect the output from one command to the input of another. <code>></code> is used to redirect standard output to a file. Try it in the <code>shell-lesson-data/molecules</code> directory!

</details>

[Episode 4 Exercise 5](episode4_ex5.md)

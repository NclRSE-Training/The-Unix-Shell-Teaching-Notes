## 7.3 Little Women

You and your friend, having just finished reading Little Women by Louisa May Alcott, are in an argument. Of the four sisters in the book, Jo, Meg, Beth, and Amy, your friend thinks that Jo was the most mentioned. You, however, are certain it was Amy. Luckily, you have a file ```LittleWomen.txt``` containing the full text of the novel (```shell-lesson-data/writing/data/LittleWomen.txt```). Using a ```for``` loop, how would you tabulate the number of times each of the four sisters is mentioned?

Hint: one solution might employ the commands ```grep``` and ```wc``` and a ```|```, while another might utilize ```grep``` options. There is often more than one way to solve a programming task, so a particular solution is usually chosen based on a combination of yielding the correct result, elegance, readability, and speed.

<details>
  <summary>
Solutions
  </summary>
  <pre><code>for sis in Jo Meg Beth Amy
do
echo $sis:
grep -ow $sis LittleWomen.txt | wc -l
done</code></pre>

Alternative, slightly inferior solution:

  <pre><code>for sis in Jo Meg Beth Amy
do
echo $sis:
grep -ocw $sis LittleWomen.txt
done</code></pre>

This solution is inferior because <code>grep -c</code> only reports the number of lines matched. The total number of matches reported by this method will be lower if there is more than one match per line.
<br>
Perceptive observers may have noticed that character names sometimes appear in all-uppercase in chapter titles (e.g. ‘MEG GOES TO VANITY FAIR’). If you wanted to count these as well, you could add the <code>-i</code> option for case-insensitivity (though in this case, it doesn’t affect the answer to which sister is mentioned most frequently).
</details>

[Episode 7 Exercise 4](episode7_ex4.md)

## 3.7 List filenames matching a pattern

When run in the molecules directory, which ls command(s) will produce this output?

```ethane.pdb methane.pdb```

1. ```ls *t*ane.pdb```
1. ```ls *t?ne.*```
1. ```ls *t??ne.pdb```
1. ```ls ethane.*```

<details>
  <summary>
Solution
  </summary>

The solution is 3.

1. shows all files whose names contain zero or more characters (<code>*</code>) followed by the letter <code>t</code>, then zero or more characters (<code>*</code>) followed by <code>ane.pdb</code>. This gives <code>ethane.pdb methane.pdb octane.pdb pentane.pdb</code>.

2. shows all files whose names start with zero or more characters (<code>*</code>) followed by the letter <code>t</code>, then a single character (<code>?</code>), then <code>ne</code>. followed by zero or more characters (<code>*</code>). This will give us <code>octane.pdb</code> and <code>pentane.pdb</code> but doesn’t match anything which ends in <code>thane.pdb</code>.

3. fixes the problems of option 2 by matching two characters (<code>??</code>) between <code>t</code> and <code>ne</code>. This is the solution.

4. only shows files starting with <code>ethane.</code>

</details>

[Episode 3 exercise 8](episode3_ex8.md)

## 7.5 ```find``` Pipeline Reading Comprehension

Write a short explanatory comment for the following shell script:

```bash
wc -l $(find . -name "*.dat") | sort -n
```

<details>
  <summary>
Solution
  </summary>

  <ol>
    <li>Find all files with a <code>.dat</code> extension recursively from the current directory</li>
    <li>Count the number of lines each of these files contains</li>
    <li>Sort the output from step 2. numerically</li>
  </ol>
</details>

[End]()

## 7.1 Using ```grep```

Which command would result in the following output:

```bash
and the presence of absence:
```

1. ```grep "of" haiku.txt```
2. ```grep -E "of" haiku.txt```
3. ```grep -w "of" haiku.txt```
4. ```grep -i "of" haiku.txt```

<details>
  <summary>
Solution
  </summary>

  The correct answer is 3, because the <code>-w</code> option looks only for whole-word matches. The other options will also match ‘of’ when part of another word.
</details>

[Episode 7 Exercise 2](episode7_ex2.md)

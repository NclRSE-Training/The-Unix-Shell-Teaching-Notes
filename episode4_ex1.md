## 4.1 What Does sort -n Do?

The file ```shell-lesson-data/numbers.txt``` contains the following lines:

```code
10
2
19
22
6
```

If we run ```sort``` on this file, the output is:

```code
10
19
2
22
6
```

If we run ```sort -n``` on the same file, we get this instead:

```code
2
6
10
19
22
```
Explain why ```-n``` has this effect.

<details>
  <summary>
Solution
  </summary>

  The <code>-n</code> option specifies a numerical rather than an alphanumerical sort.

  </details>

[Episode 4 Exercise 2](episode4_ex2.md)


## 5.7 Nested Loops

Suppose we want to set up a directory structure to organize some experiments measuring reaction rate constants with different compounds and different temperatures. What would be the result of the following code:

```bash
$ for species in cubane ethane methane
> do
>     for temperature in 25 30 37 40
>     do
>         mkdir $species-$temperature
>     done
> done
```

<details>
  <summary>
Solution
  </summary>

We have a nested loop, i.e. contained within another loop, so for each species in the outer loop, the inner loop (the nested loop) iterates over the list of temperatures, and creates a new directory for each combination.
<br>
Try running the code for yourself to see which directories are created!
</details>

[Episode 6 Exercise 1](episode6_ex1.md)

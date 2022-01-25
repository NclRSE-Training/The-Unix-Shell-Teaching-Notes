## 6.2 Why Record Commands in the History Before Running Them?

If you run the command:

```bash
$ history | tail -n 5 > recent.sh
```

the last command in the file is the ```history``` command itself, i.e., the shell has added history to the command log before actually running it. In fact, the shell always adds commands to the log before running them. Why do you think it does this?

<details>
  <summary>
Solution
  </summary>

If a command causes something to crash or hang, it might be useful to know what that command was, in order to investigate the problem. Were the command only be recorded after running it, we would not have a record of the last command run in the event of a crash.
</details>

[Episode 6 Exercise 3](episode6_ex3.md)

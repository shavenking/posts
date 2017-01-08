# Use less To Replace tail -f

Everytime we need to get updated contents from a log file, we use the following command: `tail -f some.log`

It's ok most of time, but sometimes it's inconvenient when we need to scroll backward. Luckily we can easily overcome this problem with `less` command.

```
less +F some.log
```

With `less +F`, we can **scroll forward** and keep trying to read when the end of file is reached. Additionally, we can use `/pattern` to search keywords in newly output content, which is the replacement of `tail -f some.log | grep 'something'`, the difference is that with `less` command we can always to go back to general mode and do whatever you want, and then back to scroll forward mode anytime!

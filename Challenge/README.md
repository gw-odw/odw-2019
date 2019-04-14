
# Challenge

Read the description here: https://github.com/gw-odw/odw-2019/tree/master/Challenge/CHALLENGE.md

# Solution of the challenge

The file results.md.gpg contains the correct answers to all
challenges. This file is encrypted with a password that you
can infer from the properties of Challenge 4 events.

To decrypt this file, run

```gpg -d results.md.gpg```

and enter the password.

The password is composed as follows. Imagine there are N
signals in the data of Challenge 4. 

```
Event 1 at t = XXXX s [timestamps have 4 digits]
Event 2 at t = YYYY s
...
Event N at t = ZZZZ s
```

The password is the concatenation of the first two digits
of the timestamps for all events in Challenge sorted by
increasing time, ie., **passwd = XXYY..ZZ**

Here is an example with 3 events:

```
Event 1 at t = 1364 s
Event 2 at t = 2135 s
Event 3 at t = 4328 s
```
--> **Passwd = 132143**

Find files with user setuid bit on
----

That is the "setuid" bit, which tells the OS to execute that program with the userid of its owner. This is typically used with files owned by root to allow normal users to execute them as root with no external tools (such as sudo).

```
find / -perm -u=s -type f 2>/dev/null
```

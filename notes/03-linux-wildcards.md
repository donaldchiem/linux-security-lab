# Linux Wildcards

## What I Learned

Wildcards are special characters used by the Linux shell to match multiple files and directories without typing every filename. The shell expands wildcard patterns before executing a command.

In this lesson, I learned how to use the `*` and `?` wildcards to search for files based on filename patterns.

## Commands

### *

Matches zero or more characters in a filename or directory name.

Examples:

```bash
ls *.txt
ls a*
ls apple.*
```

---

### ?

Matches exactly one character in a filename or directory name.

Examples:

```bash
ls ?.txt
ls ??.txt
ls a?.txt
```

## Key Takeaways

- `*` matches zero or more characters.
- `?` matches exactly one character.
- Wildcards are expanded by the shell before a command is executed.
- Wildcards make it easier to work with multiple files and directories.

## Summary

This lesson introduced Linux wildcards and how they simplify working with files and directories. I learned how to use the `*` and `?` wildcards to match filename patterns and how the shell expands wildcard expressions before executing commands.
# Linux Permissions

## What I Learned

Linux permissions control who can read, write, or execute files and directories. Every file and directory has permissions assigned to the owner, group, and others.

Permissions can be viewed with `ls -l` and changed using `chmod`. They can be represented using either symbolic notation (`rwx`) or numeric (octal) notation (`755`, `644`, etc.).

For directories, permissions behave differently than they do for files. The execute (`x`) permission allows a user to traverse (enter) a directory rather than execute it.

## Commands

### ls -l

Displays detailed information about files, including permissions, owner, group, size, and modification date.

```bash
ls -l
```

Example:

```bash
-rw-r--r-- 1 donald donald 0 Jul 26 14:19 permissions-practice.txt
```

### ls -ld

Displays information about the directory itself instead of listing its contents.

```bash
ls -ld permissions-dir
```

Example:

```bash
drwxr-x--- 2 donald donald 4096 Jul 26 14:27 permissions-dir
```

### chmod

Changes the permissions of a file or directory.

Symbolic example:

```bash
chmod u+x permissions-practice.txt
```

Numeric example:

```bash
chmod 755 permissions-practice.txt
```

Common permission values:

- `755` → `rwxr-xr-x` (common for directories and executable files)
- `644` → `rw-r--r--` (common for regular files)
- `600` → `rw-------` (commonly used for private files, such as SSH private keys)
- `700` → `rwx------` (commonly used for private directories)

### stat

Displays detailed information about a file, including numeric and symbolic permissions.

```bash
stat permissions-practice.txt
```

Example:

```text
Access: (0600/-rw-------)
```

## Key Takeaways

- Linux permissions are divided into owner, group, and others.
- `r` = read, `w` = write, `x` = execute (or traverse for directories).
- Files and directories interpret permissions differently.
- Permissions can be changed using either symbolic or numeric notation with `chmod`.
- `ls -l` displays permissions, while `stat` provides additional file metadata.

## Summary

This lesson introduced Linux permissions and how they control access to files and directories. I learned how to view permissions, modify them using symbolic and numeric notation with `chmod`, interpret common permission values, understand the difference between file and directory permissions, and inspect detailed file metadata using `stat`.
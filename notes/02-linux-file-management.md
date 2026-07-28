# Linux File Management

## What I Learned

Linux provides commands for copying, moving, renaming, and deleting files and directories. These commands are essential for organizing files and managing the filesystem.

In this lesson, I learned how to copy files, move and rename files, remove files, and delete empty directories using common Linux commands.

## Commands

### cp

Copies a file or directory to another location.

```bash
cp source destination
```

Example:

```bash
cp day1.txt day1-copy.txt
```

---

### mv

Moves or renames a file or directory.

```bash
mv source destination
```

Example:

```bash
mv day1-copy.txt notes.txt
```

---

### rm

Permanently deletes a file or, with the appropriate options, a directory.

```bash
rm filename
```

Example:

```bash
rm notes.txt
```

---

### rmdir

Removes an empty directory.

```bash
rmdir directory
```

Example:

```bash
rmdir practice
```

> **Note:** `rmdir` only works on empty directories. If the directory contains files or other directories, the command will fail.

## Key Takeaways

- `cp` copies files and directories.
- `mv` moves or renames files and directories.
- `rm` permanently deletes files.
- `rmdir` removes empty directories only.
- File management commands are essential for organizing the Linux filesystem.

## Summary

This lesson introduced basic Linux file management commands. I learned how to copy, move, rename, and delete files, as well as remove empty directories using common Linux commands.
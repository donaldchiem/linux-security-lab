# Linux Find & Locate

## What I Learned

Linux provides several commands for locating files, directories, and executable programs. Each command serves a different purpose depending on what you are searching for.

In this lesson, I learned how to search for files and directories using `find`, locate executable programs with `which`, and identify the locations of binaries, source files, and manual pages using `whereis`.

## Commands

### find -name

Searches for files or directories using a case-sensitive name match.

```bash
find path -name "pattern"
```

Example:

```bash
find . -name "*.txt"
```

---

### find -iname

Searches for files or directories using a case-insensitive name match.

```bash
find path -iname "pattern"
```

Example:

```bash
find . -iname "*.txt"
```

---

### find -type f

Searches only for files.

```bash
find path -type f
```

Example:

```bash
find . -type f
```

---

### find -type d

Searches only for directories.

```bash
find path -type d
```

Example:

```bash
find . -type d
```

---

### which

Displays the location of an executable command in the system's `PATH`. If the command is not found, no output is displayed.

```bash
which command
```

Example:

```bash
which bash
```

---

### whereis

Displays the locations of a command's binary, source files, and manual pages (when available).

```bash
whereis command
```

Example:

```bash
whereis bash
```

## Key Takeaways

- `find` recursively searches directories for files and directories.
- `-name` performs a case-sensitive filename search.
- `-iname` performs a case-insensitive filename search.
- `-type f` searches only for files.
- `-type d` searches only for directories.
- `which` locates the executable path of a command.
- `whereis` displays the locations of a command's binary, source files, and manual pages.

## Summary

This lesson introduced Linux file and command location tools. I learned how to search for files and directories using `find`, locate executable programs with `which`, and identify the locations of binaries, source files, and manual pages using `whereis`.
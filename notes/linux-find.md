# Linux Find & Locate

## What I Learned

### find

The `find` command searches recursively through directories for files and directories that match specific search criteria.

Examples:

```bash
find . -name "*.txt"
```

Searches for `.txt` files using a case-sensitive filename match.

```bash
find . -iname "*.txt"
```

Searches for `.txt` files using a case-insensitive filename match.

```bash
find . -type f
```

Lists only files.

```bash
find . -type d
```

Lists only directories.

---

### which

The `which` command displays the location of an executable command in your system's `PATH`.

Examples:

```bash
which ls
which find
which bash
```

---

### whereis

The `whereis` command displays the locations of a command's binary, source files, and manual pages (when available).

Examples:

```bash
whereis bash
whereis find
whereis git
```

---

## Key Takeaways

- `find` recursively searches directories for files and directories.
- `-name` performs a case-sensitive filename search.
- `-iname` performs a case-insensitive filename search.
- `-type f` searches only for files.
- `-type d` searches only for directories.
- `which` locates the executable path of a command.
- `whereis` displays the locations of a command's binary, source files, and manual pages.

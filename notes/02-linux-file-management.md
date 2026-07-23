# Linux File Management

## Copy Files (`cp`)

**Syntax:**

```bash
cp <source> <destination>
```

**Example:**

```bash
cp day1.txt day1-copy.txt
```

**What it does:**
Creates a duplicate of a file while leaving the original unchanged.

## Move / Rename Files (`mv`)

**Syntax:**

```bash
mv <source> <destination>
```

**Example:**

```bash
mv day1-copy.txt notes.txt
```

**What it does:**
Moves a file or directory to a new location, or renames it if the destination is in the same directory.

## Remove Files (`rm`)

**Syntax:**

```bash
rm <filename>
```

**Example:**

```bash
rm notes.txt
```

**What it does:**
Permanently deletes a file from the current location.

## Remove Empty Directories (`rmdir`)

**Syntax:**

```bash
rmdir <directory>
```

**Example:**

```bash
rmdir practice
```

**What it does:**
Permanently deletes an empty directory. If the directory contains files or other directories, the command will fail.

> **Note:** `rmdir` only works on empty directories.

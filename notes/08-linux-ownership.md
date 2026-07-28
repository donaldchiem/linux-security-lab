# Linux Ownership

## What I Learned

In Linux, every file and directory has an owner and a group owner. Ownership works together with file permissions to determine who can access, modify, and manage files and directories.

In this lesson, I learned how to view ownership information, change file owners, change group ownership, and recursively update ownership for entire directory structures.

## Commands

### ls -l

Displays files and directories with their permissions, owner, group owner, and other details.

```bash
ls -l
```

Example:

```bash
ls -l permissions-practice.txt
```

---

### ls -ld

Displays information about a directory itself instead of listing its contents.

```bash
ls -ld directory-name
```

Example:

```bash
ls -ld ownership-practice
```

---

### stat

Displays detailed information about a file or directory, including ownership, permissions, timestamps, and metadata.

```bash
stat file
```

Example:

```bash
stat permissions-practice.txt
```

---

### chown

Changes the owner of a file or directory.

```bash
sudo chown user file
```

Example:

```bash
sudo chown root permissions-practice.txt
```

---

### chown user:group

Changes both the owner and the group owner of a file or directory.

```bash
sudo chown user:group file
```

Example:

```bash
sudo chown donald:root permissions-practice.txt
```

---

### chgrp

Changes only the group owner of a file or directory.

```bash
sudo chgrp group file
```

Example:

```bash
sudo chgrp donald permissions-practice.txt
```

---

### chown -R

Recursively changes the owner and group owner of a directory and all of its contents.

```bash
sudo chown -R user:group directory
```

Example:

```bash
sudo chown -R root:root ownership-practice
```

## Key Takeaways

- Every file and directory has an owner and a group owner.
- Ownership and permissions work together to control access.
- `ls -l` displays ownership information.
- `stat` provides detailed ownership, permission, and timestamp information.
- `chown` changes the file owner.
- `chgrp` changes only the group owner.
- The `-R` option applies ownership changes recursively to a directory and everything inside it.

## Summary

This lesson introduced Linux ownership and the commands used to manage it. I practiced viewing ownership information, changing file owners, changing group owners, and recursively updating ownership for directories and their contents. These commands are fundamental skills for Linux administration, IT support, and cybersecurity.
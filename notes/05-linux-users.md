# Linux Users

## What I Learned

Linux uses user accounts to identify who is logged into the system and determine what resources they can access. Each user has a unique User ID (UID), belongs to one or more groups, and has account information stored in system files.

In this lesson, I learned how to identify the current user, view user account information, inspect user and group IDs, locate the home directory, and list user accounts on the system.

## Commands

### whoami

Displays the username of the current logged-in user.

```bash
whoami
```

Example:

```text
donald
```

---

### id

Displays a user's UID, GID, and group memberships.

```bash
id username
```

Example:

```bash
id donald
```

```text
uid=1000(donald) gid=1000(donald) groups=1000(donald),27(sudo)
```

---

### getent passwd

Displays information stored for a user.

```bash
getent passwd username
```

Example:

```bash
getent passwd donald
```

Fields include:

- Username
- UID
- GID
- Full name
- Home directory
- Default shell

---

### echo $HOME

Displays the current user's home directory.

```bash
echo $HOME
```

Example:

```text
/home/donald
```

---

### pwd

Displays the current working directory.

```bash
pwd
```

Example:

```text
/home/donald
```

---

### cut

Displays every user account on the system, including system accounts.

```bash
cut -d: -f1 /etc/passwd
```

Example:

```text
root
daemon
bin
sys
sync
...
```

## Key Takeaways

- Every Linux user has a unique User ID (UID).
- Every user belongs to one or more groups.
- User information is stored in `/etc/passwd`.
- Passwords are stored separately in `/etc/shadow`.
- The root user is the system administrator.

## Summary

This lesson introduced Linux users and how the operating system identifies user accounts. I learned how to identify the current user, inspect user and group information, view account details, locate the home directory, and list user accounts stored on the system.
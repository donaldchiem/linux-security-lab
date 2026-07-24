# Linux Users

## What I Learned
Learn how Linux identifies users, stores user information, and determines the currently logged-in user.

---

## Commands

### Display the current user

```bash
whoami
```

Displays the username of the current logged-in user.

Example output:

```text
donald
```

---

### Display user and group information

```bash
id
```

Displays:
- User ID (UID)
- Primary Group ID (GID)
- Groups the user belongs to

Example:

```text
uid=1000(donald) gid=1000(donald) groups=1000(donald),27(sudo)
```

---

### View user account information

```bash
getent passwd donald
```

Displays information stored for a user.

Fields include:
- Username
- UID
- GID
- Full name
- Home directory
- Default shell

---

### Display the home directory

```bash
echo $HOME
```

Example:

```text
/home/donald
```

---

### Display the current directory

```bash
pwd
```

Example:

```text
/home/donald
```

---

### List all users

```bash
cut -d: -f1 /etc/passwd
```

Displays every user account on the system, including system accounts.

---

## Key Takeaways

- Every Linux user has a unique User ID (UID).
- Every user belongs to one or more groups.
- User information is stored in `/etc/passwd`.
- Passwords are stored separately in `/etc/shadow`.
- The root user is the system administrator.

---

## Summary

Today I learned how Linux identifies users, displays user information, lists system accounts, and locates a user's home directory.
# Linux Groups

## What I Learned

Linux groups are used to organize users and simplify file and system permission management. Instead of assigning permissions to individual users, administrators can assign permissions to groups and add users to those groups. This makes managing multiple users much easier.

## Commands

### groups

Displays the groups the current user belongs to.

```bash
groups
```

Example

```text
donald adm cdrom sudo dip plugdev users lpadmin lxd
```

### cat /etc/group

Displays every group configured on the system.

```bash
cat /etc/group
```
Example

```text
sudo:x:27:donald
```

### grep

Searches for a specific group inside the group database.

```bash
grep cybersecurity /etc/group
```

### groupadd

Creates a new Linux group.

```bash
sudo groupadd cybersecurity
```

### usermod -aG

Adds a user to an existing group.

```bash
sudo usermod -aG cybersecurity donald
```

### id

Displays a user's UID, GID, and group memberships.

```bash
id
```

```bash
id donald
```
Example

```text
uid=1000(donald) gid=1000(donald) groups=1000(donald),4(adm),...
```

### groupdel

Deletes a Linux group.

```bash
sudo groupdel cybersecurity
```
Example

Deletes the `cybersecurity` group. If successful, no output is displayed.

## Key Takeaways

- Linux groups simplify permission management.
- Every group has a unique Group ID (GID).
- Users can belong to multiple groups.
- Group membership changes usually require a new login session.
- Administrative tasks often require `sudo`.

## Summary

In this lesson I learned how Linux groups work, how to view existing groups, create a new group, add a user to a group, verify group membership, and remove a group. These skills are fundamental for Linux system administration and cybersecurity.
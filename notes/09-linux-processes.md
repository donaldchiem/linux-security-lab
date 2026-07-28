# Linux Processes

## What I Learned

Linux runs programs as processes. Each process has a unique Process ID (PID) and can be monitored, filtered, paused, resumed, or terminated. I learned how to inspect running processes, identify them by PID or name, and understand the relationship between parent and child processes.

## Commands

### ps

Displays running processes.

```bash
ps
```

---

### ps -e

Displays every running process.

```bash
ps -e
```

---

### ps -ef

Shows all processes with detailed information.

```bash
ps -ef
```

---

### ps aux

Displays all running processes with CPU and memory usage.

```bash
ps aux
```

---

### ps -u

Shows processes owned by a specific user.

```bash
ps -u username
```

Example:

```bash
ps -u donald
```

---

### ps -p

Displays information for a specific Process ID (PID).

```bash
ps -p PID
```

Example:

```bash
ps -p 1
```

---

### pstree

Displays processes in a parent-child tree.

```bash
pstree
```

---

### top

Monitors processes and system resources in real time.

```bash
top
```

---

### pgrep

Finds processes by name.

```bash
pgrep process_name
```

Example:

```bash
pgrep bash
```

---

### pidof

Returns the PID of a process.

```bash
pidof process_name
```

Example:

```bash
pidof bash
```

---

### jobs

Displays background jobs started in the current shell.

```bash
jobs
```

---

### kill

Sends a signal to a process. By default, it sends the `SIGTERM` signal.

```bash
kill PID
```

Example:

```bash
kill 4556
```

## Key Takeaways

- Every running program is a process.
- Each process has a unique PID.
- `ps` is used to inspect processes.
- `pstree` shows parent-child relationships.
- `top` monitors processes in real time.
- `pgrep` and `pidof` quickly locate processes.
- `kill` sends signals such as `SIGTERM`, `SIGSTOP`, and `SIGCONT`.

## Summary

This lesson introduced Linux process management. I learned how to view, search, monitor, and control processes using common Linux commands that are essential for IT support, Linux administration, and cybersecurity.
# Linux Networking

## What I Learned

Linux networking commands allow me to inspect how my computer communicates with other devices and the internet. I learned how to view network interfaces, check IP addresses, inspect the routing table, verify internet connectivity, examine listening ports, perform DNS lookups, and display my assigned IP addresses.

## Commands

### ip address

Displays all network interfaces along with their IPv4 and IPv6 addresses.

```bash
ip address
```

---

### ip link

Displays network interfaces, their status (UP or DOWN), and link-layer (MAC) addresses.

```bash
ip link
```

---

### ip route

Displays how network traffic is routed, including the default gateway.

```bash
ip route
```

---

### cat /etc/resolv.conf

Displays the DNS resolver configuration used by the system.

```bash
cat /etc/resolv.conf
```

---

### ping

Sends ICMP echo requests to verify connectivity with another host.

```bash
ping -c count hostname_or_ip
```

Example:

```bash
ping -c 4 google.com
```

---

### ss -tuln

Displays listening TCP and UDP ports on the system.

```bash
ss -tuln
```

---

### nslookup

Looks up DNS information for a domain name.

```bash
nslookup domain
```

Example:

```bash
nslookup google.com
```

---

### dig

Displays detailed DNS information for a domain.

```bash
dig domain
```

Example:

```bash
dig google.com
```

---

### hostname -I

Displays all IP addresses assigned to the local machine.

```bash
hostname -I
```

## Key Takeaways

- `ip address` displays network interfaces and IP addresses.
- `ip link` shows network interface status and MAC addresses.
- `ip route` displays the routing table and default gateway.
- `cat /etc/resolv.conf` shows DNS resolver configuration.
- `ping` verifies internet and network connectivity.
- `ss -tuln` lists listening TCP and UDP ports.
- `nslookup` performs basic DNS lookups.
- `dig` provides detailed DNS query information.
- `hostname -I` quickly displays the system's assigned IP addresses.

## Summary

This lesson introduced Linux networking fundamentals. I learned how to inspect network interfaces, view IP addresses, examine routing information, verify internet connectivity, inspect listening services, perform DNS lookups, and retrieve my system's assigned IP addresses. These commands are essential for IT support, Linux administration, system troubleshooting, and cybersecurity.
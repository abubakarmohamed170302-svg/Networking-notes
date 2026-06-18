# Network Security & Firewalls

## What is Network Security?

Network security means:

> protecting devices, data, and traffic.

Without security:

```text
Anyone could access your systems.
```

Very dangerous.

---

## Why Network Security Matters

Protects against:

* hackers
* malware
* unauthorized access
* data leaks
* attacks

Used everywhere in DevOps.

---

## What is a Firewall?

A firewall is:

> a traffic filter.

Think:

```text
Security guard for your network
```

It decides:

```text
Allow or Block
```

traffic.

---

## Example

Traffic tries to enter:

```text
Port 22 (SSH)
```

Firewall checks:

```text
Allowed?
```

If yes:

```text
Connection accepted
```

If no:

```text
Connection denied
```

---

## Inbound vs Outbound Rules

### Inbound

Controls incoming traffic.

Example:

```text
Allow SSH on port 22
```

---

### Outbound

Controls outgoing traffic.

Example:

```text
Allow internet access on port 443
```

---

## Common Ports

Very important:

```text
22   SSH
80   HTTP
443  HTTPS
53   DNS
3306 MySQL
5432 PostgreSQL
```

Know these.

---

## Principle of Least Privilege

Only allow what is needed.

Bad:

```text
Allow all traffic
```

Good:

```text
Allow only required ports
```

Safer.

---

## Firewall Commands

Linux (UFW):

Allow SSH:

```bash
sudo ufw allow 22
```

Check status:

```bash
sudo ufw status
```

Enable firewall:

```bash
sudo ufw enable
```

---

## AWS Security Groups

In AWS:

Security Groups act like firewalls.

Example:

```text
Allow:
22 (SSH)
80 (HTTP)
443 (HTTPS)
```

Very common in DevOps.

---

## Why Firewalls Matter in DevOps

Used for:

* servers
* containers
* cloud instances
* databases
* APIs

Security starts with networking.

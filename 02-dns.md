# DNS (Domain Name System)

## What is DNS?

DNS converts:

```text id="jmfkhh"
Names → IP addresses
```

Example:

Without DNS:

```text id="36m39q"
google.com
```

would need:

```text id="tdbgvs"
142.250.x.x
```

Hard to remember.

DNS solves this.

---

## Why DNS Matters

Humans remember:

```text id="nq2j8f"
google.com
```

Machines need:

```text id="hgt0km"
IP addresses
```

DNS translates.

---

## DNS Example

You type:

```text id="h43m2w"
google.com
```

Flow:

```text id="6gqu8p"
Your PC
 ↓
DNS Server
 ↓
Find IP
 ↓
Return IP
 ↓
Connect to Website
```

---

## DNS Record Types

### A Record

Maps domain to IPv4.

Example:

```text id="vbhk12"
google.com → 142.250.x.x
```

---

### AAAA Record

Maps domain to IPv6.

---

### CNAME

Alias of another domain.

Example:

```text id="x4v4yx"
www.example.com → example.com
```

---

### MX Record

Mail servers.

Used for email.

---

### TXT Record

Stores text.

Often used for verification.

---

## Common DNS Commands

Check DNS:

```bash id="xgjl88"
nslookup google.com
```

---

More detailed:

```bash id="2rjv4l"
dig google.com
```

---

Ping domain:

```bash id="vmq2ny"
ping google.com
```

Tests connectivity.

---

## DNS Problems

Common issues:

* website not loading
* wrong IP returned
* DNS server down
* slow lookups

Troubleshooting:

```bash id="k5l4e7"
nslookup
dig
ping
```

---

## Why DNS Matters in DevOps

Used constantly for:

* websites
* APIs
* cloud services
* load balancers
* internal systems

Without DNS:

cloud becomes much harder to manage.

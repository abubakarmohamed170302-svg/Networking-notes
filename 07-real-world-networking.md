# Real World Networking

## Networking in DevOps

Networking is used every day.

Examples:

* server communication
* API communication
* cloud networking
* container networking
* load balancing

Everything connects through networking.

---

## Example: User Visits Website

Flow:

```text
User
 ↓
DNS
 ↓
Public IP
 ↓
Load Balancer
 ↓
Web Server
 ↓
Application
 ↓
Database
```

This is a real production flow.

---

## Docker Networking

Containers communicate over networks.

Example:

```text
Frontend Container
 ↓
Backend Container
 ↓
Database Container
```

Docker networking is critical.

Commands:

```bash
docker network ls
docker network inspect
```

---

## AWS Networking

Core AWS networking:

* VPC
* Subnets
* Route Tables
* Internet Gateway
* NAT Gateway
* Security Groups

These are all networking.

---

## Example AWS Flow

```text
Internet
 ↓
Internet Gateway
 ↓
Public Subnet
 ↓
Web Server
 ↓
Private Subnet
 ↓
Database
```

Very common.

---

## Kubernetes Networking

Pods communicate over IP.

Important concepts:

* pod-to-pod communication
* services
* ingress
* DNS

Networking becomes even more important.

---

## Load Balancers

Distribute traffic.

Instead of:

```text
One server overloaded
```

Use:

```text
Load Balancer
 ↓
Server 1
Server 2
Server 3
```

More reliable.

---

## Common Real World Problems

Examples:

Website down:

* DNS issue
* firewall issue
* routing issue

Server unreachable:

* wrong IP
* wrong route
* blocked port

App cannot connect to DB:

* security group
* subnet issue
* firewall rule

---

## Real World Troubleshooting Flow

Step 1:

Can I reach it?

```bash
ping
```

---

Step 2:

Can DNS resolve?

```bash
nslookup
dig
```

---

Step 3:

What path is traffic taking?

```bash
traceroute
```

---

Step 4:

Are ports open?

```bash
ss -tuln
netstat -tuln
```

---

Step 5:

Is app responding?

```bash
curl
```

---

## DevOps Truth

Most infrastructure problems involve networking.

Think:

```text
If it cannot connect,
check networking first.
```

That rule solves many problems.

---

## Golden Rule

Networking is the foundation of:

```text
Linux
Docker
AWS
Kubernetes
Cloud
Security
DevOps
```

Master networking and everything after becomes easier.

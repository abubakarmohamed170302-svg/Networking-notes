# Routing

## What is Routing?

Routing is:

> the process of moving data from one network to another.

Think:

```text id="yx27pw"
Traffic directions for data
```

Without routing:

devices could only talk inside the same network.

---

## What is a Router?

A router is:

> a device that forwards traffic.

Example:

```text id="l08mtr"
Laptop
 ↓
Router
 ↓
Internet
 ↓
Server
```

The router decides where data goes.

---

## How Routing Works

Every packet has:

* source IP
* destination IP

Router checks:

```text id="1ppj9f"
Where should this go?
```

Then forwards it.

---

## Routing Table

A routing table is:

> a list of paths.

Think:

```text id="kntr5q"
Road map
```

Example:

```text id="96v0fk"
Destination     Gateway
192.168.1.0     Local
0.0.0.0         Internet
```

---

## Default Gateway

The default gateway is:

> where traffic goes if destination is outside local network.

Usually your router.

Example:

```text id="p8f14l"
192.168.1.1
```

Very important.

---

## Basic Route Flow

Example:

```text id="6sc1f0"
PC → Router → ISP → Website Server
```

That is basic internet routing.

---

## Commands

Show routing table:

Linux:

```bash id="pdgqwm"
ip route
```

Windows:

```bash id="jpkq9a"
route print
```

Check gateway:

```bash id="zv5nq3"
ipconfig
```

---

## Why Routing Matters in DevOps

Used in:

* AWS VPCs
* Docker networks
* Kubernetes networking
* Load balancers
* VPNs

Routing is everywhere.

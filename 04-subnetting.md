# Subnetting

## What is Subnetting?

Subnetting means:

> splitting a network into smaller networks.

Think:

```text id="y92d9m"
One big office → multiple departments
```

---

## Why Use Subnetting?

Benefits:

* better organisation
* better security
* less traffic
* easier management

---

## Example Network

Without subnetting:

```text id="v0dcxv"
192.168.1.0
```

Everyone in one network.

With subnetting:

```text id="frjvsd"
192.168.1.0/26
192.168.1.64/26
192.168.1.128/26
192.168.1.192/26
```

Smaller groups.

---

## CIDR Notation

CIDR shows subnet size.

Example:

```text id="4zwbnk"
192.168.1.0/24
```

`/24` means:

```text id="v9m9eu"
255.255.255.0
```

---

## Common CIDR Sizes

```text id="0p0w9g"
/24 = 256 addresses
/25 = 128 addresses
/26 = 64 addresses
/27 = 32 addresses
```

Important to remember.

---

## Network Address

Identifies the subnet.

Example:

```text id="k38h0n"
192.168.1.0
```

---

## Broadcast Address

Sends to all devices.

Example:

```text id="vn4h18"
192.168.1.255
```

---

## Host Range

Usable IPs:

```text id="qf9kz1"
192.168.1.1 - 192.168.1.254
```

---

## Why Subnetting Matters in DevOps

Used heavily in:

* AWS VPCs
* Security groups
* Private/public subnets
* Kubernetes clusters
* Internal infrastructure

Cloud uses subnetting everywhere.

# Domain + EC2 + DNS Project

## Overview

This project connects networking fundamentals with cloud hosting.

I launched an Ubuntu EC2 instance on AWS, installed NGINX, configured Cloudflare DNS, and connected my custom subdomain to the server.

Final live domain:

https://nginx.abubakarmohamed.dev

---

## Objective

The goal of this project was to:

* Buy a custom domain
* Launch an EC2 instance
* Install NGINX
* Configure DNS records
* Connect the domain to the EC2 public IP
* Make the NGINX page load over the internet

---

## What I Built

* Ubuntu EC2 instance
* NGINX web server
* Cloudflare DNS A record
* Cloudflare SSL/TLS setup
* Public website accessible through my subdomain

---

## Architecture

Browser
↓
Cloudflare
↓
AWS EC2 Public IP
↓
NGINX Web Server

---

## Technologies Used

* AWS EC2
* Ubuntu Linux
* NGINX
* Cloudflare DNS
* SSH
* Security Groups
* HTTP / HTTPS
* GitHub

---

## Networking Concepts Practiced

### Public IP Address

The EC2 instance was assigned a public IP:

54.196.147.85

This allowed it to be reached from the internet.

---

### DNS A Record

Cloudflare DNS was configured:

nginx.abubakarmohamed.dev → 54.196.147.85

This connects the domain to the server.

---

### Ports Used

Port 22 → SSH
Port 80 → HTTP
Port 443 → HTTPS (handled by Cloudflare)

---

### Security Groups

The EC2 security group allowed:

* Port 22 from my IP
* Port 80 from anywhere

This allowed secure remote access and public website access.

---

### Cloudflare Proxy + SSL

The final working setup used:

* Proxy enabled
* SSL/TLS mode set to Flexible

Traffic flow:

Browser → HTTPS → Cloudflare → HTTP → EC2

Cloudflare handled HTTPS while EC2 served HTTP.

---

## Screenshots

The screenshots folder contains:

* EC2 running
* EC2 details
* Security group rules
* SSH connection
* Internal IP
* NGINX running
* Port 80 listening
* Cloudflare DNS
* Cloudflare SSL/TLS
* Public IP working
* Domain working

---

## Challenges Faced

### Issue: Domain was not loading

At first, the EC2 public IP worked but the domain did not.

### Troubleshooting Steps

I checked:

* Security group rules
* NGINX service
* Port listening
* DNS resolution
* Cloudflare settings

### Solution

The browser was trying HTTPS, but the server was only serving HTTP.

Fix:

* Enabled Cloudflare proxy
* Changed SSL/TLS mode to Flexible

After this, the domain loaded successfully.

---

## What I Learned

This project helped me understand:

* How EC2 hosting works
* How DNS records work
* How NGINX serves websites
* How ports control traffic
* How Cloudflare proxies traffic
* The difference between HTTP and HTTPS
* How to troubleshoot real infrastructure issues

---

## Final Result

My custom subdomain successfully serves the NGINX landing page over HTTPS:

https://nginx.abubakarmohamed.dev

---

## Reflection

This project helped connect theory to real-world infrastructure.

It showed how Linux, networking, DNS, cloud hosting, security groups, and web servers work together in a DevOps workflow.


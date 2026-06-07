# BGP Labs - iBGP, Split Horizon, and Route Reflector

## Purpose

Hands-on Cisco CML labs created to understand:

* iBGP fundamentals
* Loopback peering
* iBGP split horizon rule
* Full mesh requirement
* Route Reflector design
* Troubleshooting methodology

---

# Labs Included

## Lab 1 - Basic iBGP

Goal:

* Build first iBGP session
* Use loopback peering
* Learn update-source

Topology:

R1 -------- R2

---

## Lab 2 - iBGP Split Horizon

Goal:

Understand why routes learned from one iBGP peer are not advertised to another iBGP peer.

Topology:

R1 -------- R2 -------- R3

---

## Lab 3 - Route Reflector

Goal:

Replace full mesh design using route reflectors.

Topology:

```
    R2 (RR)
   /       \
R1(Client)   R3(Client)

---

# Verification Commands

show ip bgp summary

show ip bgp

show ip bgp neighbors

show ip route bgp

---

# Key Learning Outcomes

* Same AS = iBGP
* iBGP preserves next-hop
* update-source for loopback peering
* Split horizon behavior
* Full mesh scalability issues
* Route reflector basics

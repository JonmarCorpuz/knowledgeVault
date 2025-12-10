# Autonomous System

An AS is a network or group of IP networks and routers that are operated by a single organization that shares on coherent routing policy with the rest of the Internet

* Each AS is identified globally by a unique ASN that BGP will use to exchange routes and build AS paths between networks
* BGP treats each AS as a distinct routing domain and exchanges reachability information between ASes rather than between individual routers alone

<br>

# Autonomous System Number

An ASN is a unique numeric ID that represents a distinct network or group of IP prefixes under a single routing policy

* Allows BGP to identify which network is originating or passing on a route

<br>

## ASN Ranges

| Type | 16-bit Range | 32-bit Range | Use Case |
| --- | --- | --- | --- |
| Public ASNs | **1-64495** | **65552-4199999999 | Internet routable (Must be globally unique) |
| Private ASNs | **64512–65534** | **4200000000–4294967294** | Internal use case (*VPN*, *etc.*) |
| Documentation Examples | **64496-64511** | **65536–65551** | Never used in production (*Documentation*, *Labs*, *Training*, *etc.*) |
| Reserved | **0**, **65535** | **0**, **4294967295** | Protocol and registry purposes |

<br>

## Peer ASN

A peer ASN is the ASN of the BGP neighbor that you're trying to establish a session with

* Each peer ASN is represemted as an ASN using either the older 16-bit space or the newer 32-bit space

<br>

# Autonomous Number Paths

An AS path is the ordered list of ASes that a route advertisement has passed through from the originating AS to the current router
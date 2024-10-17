---
title: UDP
layout: home
parent: Notes
---

# UDP

## Port Numbers

- https://kak.kornev-online.net/FILES/KAK%20-%20TCP%20List%20of%20TCP%20and%20UDP%20port%20numbers.pdf

## UDP: segment header

- fixed bytes: 8 bytes
- http://ftp.cerias.purdue.edu/pub/doc/rfc/rfc768.txt

[[UDP_ICMP_Headers.pdf]]
https://www.cs.nmt.edu/~risk/UDP_ICMP_Headers.pdf

```
Format
------

                                    
                  0      7 8     15 16    23 24    31  
                 +--------+--------+--------+--------+ 
                 |     Source      |   Destination   | 
                 |      Port       |      Port       | 
                 +--------+--------+--------+--------+ 
                 |                 |                 | 
                 |     Length      |    Checksum     | 
                 +--------+--------+--------+--------+ 
                 |                                     
                 |          data octets ...            
                 +---------------- ...                 

                      User Datagram Header Format
```

## TCP 3-way handshake

- client state
	- LISTEN -> SYNSENT -> ESTAB
- server state
	- LISTEN -> SYN RCVD -> ESTAB

![[handshake.png]]



---

Last Updated: Thu Oct 17 11:00:48 CST 2024

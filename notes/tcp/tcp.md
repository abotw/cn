---
title: TCP
layout: home
parent: Notes
---

# TCP

Connection-oriented Transport: TCP

## Readings

- Post: [计算机网络 - TCP 协议原理总结](https://writings.sh/post/network-tcp)
- https://phoenix.goucher.edu/~kelliher/s2011/cs325/mar21.html
- https://cs.nyu.edu/~jcf/classes/g22.2262-001_sp11/slides/session9/TheInternetTransportProtocols-TCP&UDP.pdf
- https://web.cs.unlv.edu/jh/CSC465/Resources/ch12.pdf
- https://www.cse.wustl.edu/~jain/cse473-21/ftp/i_3tcp.pdf
- https://www.albany.edu/faculty/dsaha/teach/2020Spring_ECE416/slides/04_transport.pdf
- https://kak.kornev-online.net/FILES/KAK%20-%20TCP%20List%20of%20TCP%20and%20UDP%20port%20numbers.pdf
- https://www.cs.memphis.edu/~xgao1/teaching/comp7327/ppt_5.pdf
- https://users.cs.jmu.edu/bernstdh/web/common/lectures/summary_tcp.php
- https://www.cs.rochester.edu/~kshen/csc257-fall2007/lectures/lecture12-tcp.pdf
- https://www.albany.edu/faculty/dsaha/teach/2020Spring_ECE416/slides/04_transport.pdf
- https://www.cs.umd.edu/~shankar/417-F01/Slides/chapter3b/tsld002.htm

## TCP segment structure

![[Pasted image 20241017101809.png]]
src: https://www.cs.umd.edu/~shankar/417-F01/Slides/chapter3b/sld002.htm

- 固定首部：20 bytes
- source port
- dest port
- counting by bytes of data (not segments!
	- **sequence number**
	- **acknowledgement number**
- **head length**
- ACK
- SYN
- FIN

## TCP 3-way handshake

- client state
	- LISTEN -> SYNSENT -> ESTAB
- server state
	- LISTEN -> SYN RCVD -> ESTAB

连接建立状态
![[handshake.png]]
- choose init `seq` num, x send TCP SYN msg
- choose init `seq` num, y send TCP SYNACK msg, acking SYN
- received SYNACK(x) indicates server is live; send ACK for SYNACK; this segment may contain client-to-server data
- received ACK(y) indicates client is live

- ack: acknowledgement number
- ACK

## TCP: closing a connection

- client, server each close their side of connection
	- send TCP segment with FIN bit = 1
- respond to received FIN with ACK
	- on receiving FIN, ACK can be combined with own FIN Ø
- simultaneous FIN exchanges can be handled

![[Pasted image 20241017113931.png]]

## TCP State Transition Diagram

![[Pasted image 20241017114042.png]]

## Principles of Congestion Control

- **congestion**
	- Informally: “too many sources sending too much data too fast for *network* to handle”
	- Different from flow control!
	- Manifestations:
		- lost packets (buffer overflow at routers)
		- long delays (queueing in router buffers)

## 拥塞控制的方法

- 开环控制
	- 事先设计
- 闭环控制
	- 反馈环路
		- 监测网络系统
		- 转移拥塞信息
		- 调整网络系统
	- 反馈形式
		- 显式反馈
			- 拥塞点 -> 源端
		- 隐式反馈
			- 自己发现

## CWND, Congestion Window, 拥塞窗口

TCP maintains a new state variable for each connection, called CongestionWindow, which is used by the source to limit how much data it is allowed to have in transit at a given time. 
§ The congestion window is congestion control’s counterpart to flow control’s advertised window. 
§ TCP is modified such that the maximum number of bytes of unacknowledged data allowed is now the minimum of the congestion window and the advertised window
- 发送方的主动控制

## Mechanisms of Adjusting cwnd

Ø A lost segment implies congestion § sender’s rate should be decreased when a segment is lost Ø ACK indicates that there is no congestion § sender’s rate can be increased when an ACK

## rwnd, 接收窗口

---

Last Updated: Thu Oct 17 10:11:39 CST 2024

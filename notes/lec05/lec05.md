---
title: "Lec 05:"
layout: home
parent: Notes
---

# Lec 05:

## DHCP

- 广播 IP 目的地址：`255.255.255.255`
- 源 IP 广播地址：`0.0.0.0`
- DHCP 服务器端口：67
- (discover, offer), request, ack

### DHCP 中继代理 (Relay Agent)

- 以单播方式发向 DHCP Server
- 可以减少 DHCP Server 的数量

### Lease Period, 租用期

- decided by the DHCP server

## P2P

- P2P vs. C/S
- find and download
- 分片，等长数据块，对等方互相交换

### 集中式目录

- 集中式目录服务器主要负责查询，不承担下载压力
	- IP地址
	- 共享资源的名称（地址）
- 降低了负载
- 但是抗风险性比较小

### 查询洪泛

- 大大增加查询的时间的成本
- 限制查询次数或查询时间，防止无限查找

## 3.1 Transport Layer Overview

- 应用层：资源子网（面向信息处理，用户功能）
- 在资源子网和通信子网中提供**桥梁**的功能，承上启下
- 网络通信实际上是进程通信
- 传输层：端口（对应业务进程）
- 同层之间的逻辑通信
- 对等层，逻辑通信，相同功能
- **端到端的通信**
- 传输层
	- 复用
	- 分用
- 网络层：点到点的通信
- 应用层：报文
- TCP、UDP：提供进程之间的逻辑通信（强调在应用层）
- IP：提供主机之间的逻辑通信（物理）
- **报文：差错检测（UDP、TCP）**

常用功能：
1. 可靠数据传输
2. 流量控制
3. 拥塞控制

- PDU (Protocol Data Unit)
- TPDU (Transport Protocol Data Unit)
- TCP Segment

- bits
- frames
- datagrams
- segments
- message

- TCP 不支持广播、多播，端对端

- 全双工 / 半双工 / 单工

### Multiplexing/demultiplexing

- 端口就是传输层的地址
- 端口：16 bits 端口号
	- 熟知端口 0-1023（用于服务器端）
	- 登记端口 1024-49151
	- 动态端口 49152-65535

## 3.2 UDP

- IP + 端口 + 差错检测
- User Datagram （基于 IP 的数据报）
- 面向报文
	- 不会再分组、也不会再合并
	- 需要 app 选择合适的报文大小
	- ==是否需要大小一致的 UDP 报文？==
- **首部**开销：8 bytes
	- **源端口 2**
	- **目的端口 2**
	- **长度 2**
		- 整个长度：首部+数据
	- **校验和 2**
- TCP首部开销：20 bytes
- 伪首部用来计算校验和
- UDP -> IP
- ==ICMP==包 （网络层）

---

Last Updated: Thu Oct 10 10:25:14 CST 2024

# FCP — Fast Channel Protocol

## Concept

FCP (Fast Channel Protocol) is a decentralized peer-to-peer file transfer protocol designed to maximize simultaneous transfers instead of dedicating the full bandwidth to a single file.

Unlike traditional transfer systems where one transfer monopolizes the available bandwidth, FCP dynamically splits the connection into multiple independent channels.

Example:

- Available bandwidth: `100 Mb/s`
- FCP channel size: `1 Mb/s`
- Maximum simultaneous transfers: `100`

Each file transfer receives its own dedicated bandwidth slice.

---

# Core Philosophy

Traditional protocols:

```txt
100 Mb/s
┌──────────────────────┐
│      File A only     │
└──────────────────────┘

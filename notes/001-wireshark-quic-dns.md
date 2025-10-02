# Lab 001 — QUIC/HTTP3 & DNS on my hotspot

**Date:** 2025-10-02  
**Goal:** Capture my own traffic safely and identify DNS + QUIC (HTTP/3).

## Setup
- Device: Laptop on personal mobile hotspot
- Tool: Wireshark + Npcap
- Scope: My traffic only

## Steps
1) Start capture on Wi-Fi interface.
2) Open a site / short music stream.
3) Stop after ~60s.
4) View **Statistics → Protocol Hierarchy**.
5) Filters: `dns`, `quic`, `tls`, `arp`.

## Findings
- QUIC dominated (UDP): ~75% packets.
- DNS resolved service domains → server IPs.
- TLS handshakes present; SNI confirms hostnames.

## Screenshots
![Protocol Hierarchy](../images/lab001-protocol-hierarchy.png)
![DNS Queries](../images/lab001-dns.png)

## Security notes
- Public IP/MAC redacted in images.
- No third-party traffic captured.

## Next
- Try TLS decryption with SSLKEYLOGFILE (own browser).
- Practice ARP analysis on a lab network.

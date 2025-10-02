# cybersecurity-learning
# Wireshark Learning Labs

Hi, I'm Belinda Tanatswa Mandudzo. This repo documents my practical journey into network traffic analysis with Wireshark.

## What I’m practicing
- Safe packet capture on my own hotspot
- Reading IPv4 headers (src/dst, TTL, protocol)
- Protocol Hierarchy to spot TLS, QUIC (HTTP/3), DNS, ARP
- Using display filters: `dns`, `tls`, `quic`, `arp`, `tcp.flags.syn == 1 && tcp.flags.ack == 0`
- Basic threat hints: DNS anomalies, ARP spoofing patterns, unusual scans

## Structure
- `notes/` – markdown lab writeups
- `images/` – redacted screenshots
- `captures/` – small, sanitized `.pcapng` samples (optional)

## Safety
Screenshots are redacted (public IPs/MACs hidden). Any pcaps are short and sanitized.

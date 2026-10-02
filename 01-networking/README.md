# 01 · Networking

Covers IP addressing and subnetting, the OSI model, TCP/UDP, DNS, NAT, firewalls, HTTP, TLS certificates and reverse proxies.

| Lab | Level | What I built / learned | File(s) | Done |
|---|---|---|---|---|
| 1.1 | 🟢 | Read my own network: IPs, masks, CIDR, NAT | `lab-1.1-my-network.md` | ⬜ |
| 1.2 | 🟡 | Production VPC IP plan (3 envs, 3 AZs, 3 tiers) | `lab-1.2-vpc-ip-plan.md` | ⬜ |
| 1.3 | 🔴 | **Subnet calculator** in Python (split, overlap check, AWS reserved IPs) | `subnet_calc.py` | ⬜ |
| 2.1 | 🟢 | DNS lookups, listening ports, port tests | `lab-2.1-dns-ports.md` | ⬜ |
| 2.2 | 🟢 | DNS from the root with `dig +trace`, all record types | `lab-2.2-dns-trace.md` | ⬜ |
| 2.3 | 🟡 | Capture the TCP handshake with tcpdump | `lab-2.3-tcp-handshake.md` | ⬜ |
| 2.4 | 🟡 | TCP connection states (TIME_WAIT, CLOSE_WAIT) | `lab-2.4-tcp-states.md` | ⬜ |
| 2.5 | 🔴 | **Network health checker** (DNS + port + latency, CI-ready exit codes) | `netcheck.py` / `netcheck.sh` | ⬜ |
| 3.1 | 🟢 | HTTP with curl: headers, status codes, timing breakdown | `lab-3.1-http-basics.md` | ⬜ |
| 3.2 | 🟢 | Inspect real TLS certificates and chains with openssl | `lab-3.2-certificates.md` | ⬜ |
| 3.3 | 🟡 | My own HTTPS server with a self-signed cert | `https_server.py` | ⬜ |
| 3.4 | 🟡 | Nginx reverse proxy; reproduce 502 and 504 | `lab-3.4-reverse-proxy/` | ⬜ |
| 3.5 | 🔴 | **TLS certificate expiry monitor** (warn/expired, exit codes, JSON, Slack) | `cert_monitor.py` | ⬜ |

| 4.1 | 🟢 | Nginx round-robin across 3 backends | `lab-4-load-balancing/nginx.conf` | ⬜ |
| 4.2 | 🟡 | LB algorithms (weight, ip_hash), passive health, backup servers, 502 on total failure | `lab-4-load-balancing/README.md` | ⬜ |
| 4.3 | 🟡 | HAProxy active health checks + stats dashboard | `lab-4-load-balancing/haproxy.cfg` | ⬜ |
| 4.4 | 🔴 | **My own load balancer in Python** (round robin / least connections, health checks, 502/503) | `lab-4-load-balancing/mini_lb.py` | ⬜ |
| 4.5 | 🔴 | AWS ALB: path rules, target groups, weighted canary (optional, delete afterwards) | `lab-4-load-balancing/lab-4.5-aws-alb.md` | ⬜ |

Lab instructions are in my lesson notes (Lessons 1–4).

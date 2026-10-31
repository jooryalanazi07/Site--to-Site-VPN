# Site-to-Site IPsec VPN

Network Security course project (Cisco Packet Tracer).

## Overview
A site-to-site IPsec VPN that creates an encrypted tunnel between two remote sites (HQ Riyadh and a remote branch) over an ISP network, so traffic between them and an internal database server stays protected.

## What I did
- Designed a WAN topology with three Cisco 2911 routers (HQ, ISP, remote site) and configured IP addressing and static default routing.
- Configured IPsec with IKE/ISAKMP (Phase 1 and 2), AES encryption, SHA-HMAC integrity, Diffie-Hellman Group 2, a pre-shared key, and a crypto map with an ACL defining the protected traffic.
- Verified the tunnel with show crypto isakmp sa and show crypto ipsec sa, and tested end-to-end access through it.
- Troubleshot a missing securityk9 license, a subnet overlap, and crypto map ordering errors.

## Files
- National_VPN_Vault_edited.pdf: full project report (design, configuration, testing, reflection)
- VPN-Project.pkt: Packet Tracer file (open with Cisco Packet Tracer)

## Tools
Cisco Packet Tracer, Cisco IOS CLI

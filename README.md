# High Availability Enterprise Headquarters Network

## Executive Summary
Enterprise campus network focused on resiliency, redundancy, and business continuity. The solution implements HSRP gateway redundancy, EtherChannel, STP optimization, VLAN segmentation, and failover validation.

## Business Impact
- Eliminates single points of failure
- Provides gateway redundancy using HSRP
- Increases bandwidth and resiliency with EtherChannel
- Prevents Layer 2 loops using STP
- Supports departmental segmentation and scalability

## Architecture
```text
                         Backup Switch
                               |
                         Main Switch
                         || EtherChannel ||
                    _____/             \_____
                   /                         \
          First Floor Dist.           Second Floor Dist.
              /      \                  /          \
        HR VLAN10  IT VLAN20   Finance VLAN30  Sales VLAN40
```

## Technologies
HSRP • EtherChannel (LACP) • STP • VLANs • 802.1Q Trunking • High Availability

## Validation
- HSRP Active Gateway Verified
- HSRP Failover Successfully Tested
- EtherChannel Operational
- STP Root Bridge Verified
- Trunking and VLAN Propagation Confirmed

## Screenshots
See screenshots folder for detailed verification evidence.

## Skills Demonstrated
Enterprise Networking, High Availability, HSRP, EtherChannel, STP, VLAN Design, Trunking, Troubleshooting, Cisco IOS.

## Author
Yash Barak

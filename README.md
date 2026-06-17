![Cisco](https://img.shields.io/badge/Cisco-Packet_Tracer-blue)
![HSRP](https://img.shields.io/badge/HSRP-Configured-success)
![EtherChannel](https://img.shields.io/badge/EtherChannel-LACP-success)
![STP](https://img.shields.io/badge/STP-Validated-success)
![CCNA](https://img.shields.io/badge/CCNA-Level_Project-orange)

# High Availability Enterprise Headquarters Network

![Banner](/screenshots/Banner2.jpeg)
 
## Executive Summary
Enterprise campus network focused on resiliency, redundancy, and business continuity. The solution implements HSRP gateway redundancy, EtherChannel, STP optimization, VLAN segmentation, and failover validation.

## Project Objectives

The primary objective of this project was to design, implement, and validate a highly available enterprise campus network capable of maintaining connectivity during infrastructure failures.

Key goals included:

* Implement gateway redundancy using HSRP
* Increase resiliency through EtherChannel
* Prevent Layer 2 loops using STP
* Segment departments using VLANs
* Validate failover behavior through testing
* Develop enterprise troubleshooting skills


## Business Value

This project was designed to simulate a highly available enterprise headquarters network capable of maintaining business operations during infrastructure failures.

The design achieves this through:

- HSRP gateway redundancy eliminating single points of failure
- EtherChannel link aggregation providing increased bandwidth and resiliency
- STP root bridge optimization preventing Layer 2 loops
- VLAN segmentation improving security and traffic isolation
- Redundant switching paths ensuring continuous connectivity

As a result, the network can continue operating during simulated gateway and link failures while maintaining access to critical business resources.

## Network Topology

![Network Topology](screenshots/topology.png)

*Figure 1: High Availability Enterprise Headquarters Network Architecture featuring HSRP gateway redundancy, EtherChannel link aggregation, STP optimization, VLAN segmentation, redundant switching paths, and enterprise failover validation.*

## Technologies
HSRP • EtherChannel (LACP) • STP • VLANs • 802.1Q Trunking • High Availability

## Validation Results

| Technology    | Verification Method              | Result                            |
| ------------- | -------------------------------- | --------------------------------- |
| HSRP          | show standby brief               | Active gateway verified           |
| HSRP Failover | Simulated VLAN interface failure | Backup switch assumed Active role |
| EtherChannel  | show etherchannel summary        | LACP operational                  |
| STP           | show spanning-tree vlan 10       | Root bridge verified              |
| Trunking      | show interfaces trunk            | VLAN propagation confirmed        |


## Key Validation Evidence

### HSRP Active State

![HSRP Active](screenshots/hsrp-active.png)

### HSRP Failover

![HSRP Failover](screenshots/hsrp-failover.png)

### EtherChannel Validation

![EtherChannel](screenshots/etherchannel-summary.png)

## Lessons Learned

During implementation and testing, several key networking concepts became clear:

### High Availability Requires Validation

Configuring HSRP is only the first step. Actual failover testing is necessary to confirm redundancy works as expected.

### EtherChannel Improves More Than Bandwidth

Link aggregation not only increases throughput but also provides resiliency if individual links fail.

### STP Design Matters

Improper root bridge placement can lead to inefficient forwarding paths and slower convergence.

### Troubleshooting Builds Real Understanding

Resolving VLAN propagation issues, trunking inconsistencies, and HSRP state transitions provided deeper insight into enterprise switching behavior.

### Documentation Is Critical

A network is only valuable if its design, validation, and troubleshooting processes can be clearly communicated to other engineers.

## Skills Demonstrated
Enterprise Networking, High Availability, HSRP, EtherChannel, STP, VLAN Design, Trunking, Troubleshooting, Cisco IOS.

## Conclusion

This project demonstrates enterprise networking concepts commonly used in production environments, including redundancy, resiliency, failover validation, and Layer 2 optimization.

Through the implementation of HSRP, EtherChannel, STP, VLAN segmentation, and structured troubleshooting, the network was designed to maintain service availability while minimizing operational risk during simulated failures.


## Author
Yashjeet Barak

# Hierarchical Topology for Language Model Coordination

IETF Internet-Draft: `draft-williams-netmod-lm-hierarchy-topology-00`

## Overview

This repository contains the development of an IETF Internet-Draft that defines a YANG data model for hierarchical coordination of distributed language models (LMs). The model enables tiny, small, and large LMs to cooperate securely across edge-to-cloud environments.

## Repository Structure

<pre>
├── draft-williams-netmod-lm-hierarchy-topology-00.txt    # Latest I-D text
├── yang/                                                 # YANG modules
│   └── ietf-lm-hierarchy@2025-07-06.yang                 # Main data model
├── examples/                                             # Usage examples
│   ├── basic-node-config.json                            # Single node configuration
│   ├── inference-request.json                            # RPC request example
│   └── multi-tier-topology.json                          # Complete hierarchy setup
├── implementation/                                       # Reference implementations
│   └── README.md                                         # UniLoRa prototype status
├── docs/                                                 # Additional documentation
│   └── use-cases.md                                      # Detailed use cases
└── .github/workflows/                                    # CI/CD automation
    └── validate.yml                                      # YANG validation
</pre>

## Quick Start

### Viewing the Draft
- Latest version: [draft-williams-netmod-lm-hierarchy-topology.txt](draft-williams-netmod-lm-hierarchy-topology.txt)
- IETF Datatracker: [Coming soon]
- HTML version: [GitHub Pages link when available]

### YANG Model
- Main module: [ietf-lm-hierarchy@2025-07-06.yang](yang/ietf-lm-hierarchy@2025-07-06.yang)
- Validation: Passes `pyang --ietf` checks
- Dependencies: `ietf-inet-types`, `ietf-yang-types`

## Key Features

- Hierarchical Architecture:** Three-tier LM coordination (tiny/small/large)
- Security: Token-based authentication with pluggable validation
- Escalation: Smart request forwarding up the hierarchy
- Health Monitoring: Heartbeat notifications for distributed systems
- Extensible: Modular trust mechanisms and validation backends

## Implementation Status

Prototype: UniLoRa Mesh LM Hierarchy
- Platform: ESP32 (Tiny LMs) → Raspberry Pi (Small LMs) → Cloud (Large LM)
- Transport: LoRa mesh networking
- Status: Early prototype, active development
- License: Apache 2.0

## Contributing

This is an active IETF Internet-Draft under development. Contributions welcome!

### How to Help:
1. Review the draft - Open issues for technical feedback
2. Test the YANG model - Try with your NETCONF/RESTCONF setup
3. Suggest use cases - What scenarios should we cover?
4. Security review - Help us strengthen the security model

### Feedback Methods:
- GitHub Issues: Technical feedback, bugs, suggestions
- Pull Requests: Specific text changes, YANG improvements  
- Email: NETMOD working group discussion (netmod@ietf.org)
- IETF Meetings: Present at NETMOD sessions

## IETF Process

- Working Group: [NETMOD](https://datatracker.ietf.org/wg/netmod/)
- Current Status: Individual draft, seeking WG adoption
- Next Steps: Present to NETMOD, incorporate feedback, iterate

## License

This Internet-Draft and associated code are provided under the BSD 3-Clause License. See [LICENSE](LICENSE) for details.

## Contact

Author: Keenan Williams  
Email: telesis001@icloud.com  
IETF Datatracker: (https://datatracker.ietf.org/doc/draft-williams-netmod-lm-hierarchy-topology/)

---

### Related Standards
- [RFC 7950](https://tools.ietf.org/html/rfc7950) - YANG 1.1 Data Modeling Language
- [RFC 8345](https://tools.ietf.org/html/rfc8345) - Network Topologies Data Model  
- [RFC 8407](https://tools.ietf.org/html/rfc8407) - YANG Module Guidelines

### Star this repo if you find it useful!

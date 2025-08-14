# NostrEx

**Note:** This project is in the early planning and development stages. We're excited about building a robust set of Elixir libraries for the Nostr protocol, and this README outlines our vision and roadmap. Contributions and feedback are welcome as we kick things off!

## About the Project

NostrEx is an upcoming open-source suite of Elixir libraries aimed at empowering developers to build decentralized applications on the Nostr protocol—a censorship-resistant framework for social networking, messaging, and more. By leveraging Elixir's BEAM VM, NostrEx will provide modular tools for seamless Nostr integration, focusing on concurrency, fault-tolerance, and extensibility.

This project addresses the need for native Elixir tooling in the Nostr ecosystem, where current options are limited. Once developed, it will enable everything from simple clients to advanced hardware-integrated devices, all while promoting open-source principles.

The libraries will be published on Hex.pm under the BSD 3-Clause License, with comprehensive documentation and examples to lower the entry barrier for Elixir developers.

## Planned Features

- **Core Modules**: Event creation, parsing, and handling; cryptographic utilities for signing and verification using secp256k1.
- **Relay and Client Support**: WebSocket-based communication for connecting to relays, subscribing to filters, and broadcasting events.
- **NIP Compliance**: Aim for comprehensive support of Nostr Improvement Proposals (NIPs), starting with the most essential ones and expanding towards full coverage. Priority on key NIPs including NIP-01 (basic protocol flow), NIP-02 (contact lists), NIP-04 (encrypted direct messages), NIP-05 (identity verification), NIP-09 (event deletion), NIP-19 (bech32-encoded entities), NIP-25 (reactions), and others such as NIP-11 (relay information), NIP-42 (relay authentication), NIP-57 (Lightning zaps), NIP-65 (relay list metadata).
- **Concurrency and Scalability**: Utilize Elixir's lightweight processes for efficient multi-relay handling and supervision trees for reliability.
- **Developer Tools**: CLI utilities, testing frameworks, and benchmarks to compare with other Nostr implementations.

## Roadmap

We're starting from scratch and aiming for a structured, milestone-based approach over 12 months, with part-time development. Progress will be tracked publicly via GitHub issues and projects. Here's the high-level plan:

1. **Months 1-3: Foundations (MVP)**  
   - Set up the repository structure, CI/CD, and testing framework.  
   - Implement core event structs and crypto utilities.  
   - Basic NIP-01 support with examples.  
   - Deliverable: Initial commit with alpha code; publish to Hex.pm as v0.1.

2. **Months 4-6: Relay/Client Core**  
   - Add WebSocket relay integration (using WebSock or Phoenix Channels).  
   - Support for NIP-05 and NIP-19.  
   - Prototype a simple client.  
   - Deliverable: Beta release; basic usage docs and examples.

3. **Months 7-9: NIP Expansions and Enhancements**  
   - Expand to additional key NIPs (e.g., NIP-02 for contact lists, NIP-04 for encrypted DMs, NIP-09 for deletions, NIP-25 for reactions).  
   - Add advanced event handling and multi-relay features.  
   - Implement benchmarks and optimizations.  
   - Deliverable: v1.0 release; comprehensive tutorials.

4. **Months 10-12: Community Focus and Full Coverage**  
   - Incorporate feedback and add more NIPs (e.g., NIP-11, NIP-42, NIP-57, NIP-65) towards full NIP support.  
   - Host workshops/AMAs on Nostr or Elixir forums.  
   - Optimize for production use and security audits.  
   - Deliverable: Refined ecosystem; aim for contributors and adopters.

We welcome early contributions! For questions, reach out on Nostr or open an issue! 🚀

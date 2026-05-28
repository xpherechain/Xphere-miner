# XPHERE Miner

> ## ⚠️ Important Notice — End of Official Miner Distribution
>
> With the activation of the **xpHash** hard fork, **official distribution of the XPHERE Miner binary has been discontinued**.
>
> This repository is preserved for historical reference. No further releases of the official miner client will be published. The XPHERE network itself continues to operate normally — only the first-party miner distribution has ended.

---

## Background

XPHERE's transition to **xpHash**, a Proof-of-Work algorithm purpose-built for the XPHERE network, marks a significant evolution of the Proof Chain. As part of this evolution, the XPHERE Foundation has discontinued the distribution of the official miner client.

This decision is deliberate, strategic, and aligned with the long-term direction of the network. The sections below explain the reasoning in detail.

---

## Why the Official Miner Is No Longer Distributed

### 1. A Specialized Mining Environment for xpHash

xpHash mining is conducted through hardware and operational setups specifically engineered for the algorithm's computational characteristics. A general-purpose, Foundation-distributed binary — as the legacy XPHERE Miner was — would not reflect the realistic mining environment of the post-fork network, and would mislead participants regarding actual mining economics, performance expectations, and operational requirements.

Continuing to publish a generic client that no longer represents how mining is actually performed would do operators a disservice. The Foundation therefore refrains from issuing such a binary and allows the mining environment to evolve on its own operational terms.

### 2. Decentralization of the Mining Layer

A single first-party binary inevitably becomes a monoculture — concentrating implementation risk, supply-chain risk, and protocol influence on one party. This contradicts the core decentralization principles that XPHERE's dual-chain architecture is designed to uphold.

By removing the official miner from the distribution path, the Foundation eliminates itself as a privileged actor in the mining stack. This separation prevents any conflict of interest between protocol stewardship and mining-side participation, and ensures that the Foundation does not occupy a structural advantage within the mining economy.

### 3. Maturation of the Network

During the early SHA-256 era of XPHERE, the official miner served as a **bootstrap mechanism** that lowered the barrier to participation and helped establish the initial hash power required to secure the network.

With the network now matured, the Proof Chain stabilized, and a sustainable validator ecosystem in place, that bootstrap role is no longer necessary. Mining is now treated as a third-party concern, in line with how mature Proof-of-Work networks operate.

### 4. Separation of Responsibilities

The Foundation's protocol engineering effort is now fully focused on:

- The Proof Chain reference node implementation
- The xpHash protocol specification and conformance
- Main Chain consensus, validator coordination, and overall network health

Mining client development falls outside this scope and is best served by **specialist teams** who can optimize for specific hardware profiles, operating systems, and operational workflows. Separating these responsibilities improves the quality of both.

### 5. Security and Supply-Chain Considerations

Centralized distribution of pre-built mining binaries creates a non-trivial supply-chain attack surface. Eliminating the official binary distribution channel removes this surface entirely.

Responsibility for binary integrity now lies with operators and third-party implementers, who can apply their own auditing, signing, and reproducible-build practices — practices typically stronger than what a single upstream distribution can provide.

### 6. Algorithmic Transition

The legacy XPHERE Miner was built against the **SHA-256** Proof-of-Work interface, which is no longer valid at and beyond the xpHash activation height. Any binary published from this repository prior to the fork is, by protocol design, unable to produce valid blocks on the post-fork chain. Continuing to host such artifacts as if they were operational software would be misleading.

---

## What This Means for Participants

- **The XPHERE network continues to operate normally.** Block production, validation, and reward distribution proceed without interruption under xpHash.
- **Mining itself is not discontinued.** What has ended is the Foundation's distribution of a generic miner binary; mining continues through the specialized environment now appropriate to xpHash.
- **Pool operations and mining services** continue independently of the Foundation. Participants who wish to mine should engage with the broader mining environment rather than rely on a first-party binary.
- **Legacy SHA-256 miner binaries** previously distributed from this repository will **not** function against post-fork heights and must not be relied upon.

---

## For Existing Operators

Operators who previously ran the official miner against the legacy SHA-256 endpoints should:

1. **Stop running the legacy binary** against any XPHERE network at or beyond the xpHash activation height.
2. **Transition to an xpHash-compatible mining setup** prior to the mainnet activation height (block `1,740,000`) through the appropriate channels for their operational profile.
3. **Confirm xpHash compatibility** with their pool operator or mining service provider, where applicable.

Continued operation of the legacy binary against post-fork heights will result in rejected submissions and wasted computational effort.

---

## Participating in Mining

Mining on xpHash is performed through the specialized mining environment that has formed around the algorithm. Operators interested in participating in mining are advised to engage with that environment directly — including their pool operator, hardware provider, or designated mining service — rather than expect a first-party client from the Foundation.

The Foundation does not maintain a public registry of mining hardware, mining software, or mining service providers, nor does it endorse any specific commercial entity. Operators are responsible for evaluating their own mining setup, counterparty risk, and operational suitability.

For general guidance on participating in the XPHERE network, please reach out through the official channels listed at the end of this document.

---

## Repository Status

This repository is retained for historical and informational purposes only.

- No further releases will be tagged.
- No further support is provided for any binary previously released here.
- Issue and pull request activity is no longer actively monitored.

For protocol-level matters, please direct inquiries to the official XPHERE channels.

---

## Network Resources

- **XPHERE Network**: <https://x-phere.com>
- **ZIGAP Wallet**: <https://about.zigap.io>
- **TestNet Faucet**: <https://faucet.x-phere.com>

---

## Contact

For protocol-level questions, please contact the XPHERE Foundation through the official channels listed on <https://x-phere.com>.

Inquiries regarding third-party miner implementations, pool operations, or hardware configuration should be directed to the respective implementers and operators.

---

*The XPHERE Foundation thanks every miner who participated in securing the network during the SHA-256 era. Your contribution made this evolution possible.*

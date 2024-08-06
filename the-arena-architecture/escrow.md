---
description: Ensuring Fair and Transparent Fund Management
---

# Escrow

The escrow system is a cornerstone of Arena DAO's competition platform, ensuring fair and transparent management of funds and assets. It provides a secure and reliable way to handle participant contributions, prize distributions, and withdrawals.

### Key Functions

#### 1. Funding

* **Multi-Token Support**: The escrow system is designed to handle multiple token types, including:
  * CW20 tokens (fungible tokens)
  * Native tokens (e.g., ATOM, OSMO)
  * CW721 tokens (non-fungible tokens, or NFTs)
* **Locking Mechanism**: Participants must send their required contributions to the escrow, which locks the funds once the competition is fully funded. This ensures that all necessary funds are secured for the duration of the competition.
* **Withdrawal**: Users can withdraw their funds from the escrow when it is in an unlocked state, typically after the competition has concluded and the distribution process is complete.

#### 2. Fund Distribution

The escrow system employs a flexible distribution mechanism to accommodate various competition structures and payout schemes:

**a. Member-Percentage Distribution**

* Funds are allocated to participants based on a predefined member-percentage list.
* The sum of all percentages must equal 100% to ensure a complete and accurate distribution.

**b. Remainder Address**

* A designated remainder address receives any leftover funds after the member share calculations have been performed.
* Due to their indivisible nature, all NFTs (CW721 tokens) are sent to the remainder address.

**c. Preset Distributions**

* Members can establish preset distribution rules for incoming funds, simplifying the distribution process.
* For example, a DAO can specify an even distribution among its members, automatically splitting the funds according to the preset rules.
* Important: Preset distributions cannot be modified once the escrow is in a locked state.

#### 3. Withdrawal Process

* After the fund distribution has been completed, users can withdraw their allocated balances from the escrow.
* The withdrawal process is initiated by the user and executed by the smart contract, ensuring a secure and auditable transfer of funds.

### Escrow States

The escrow system has two primary states:

1. **Unlocked**: In this state, the escrow is ready to receive funds and allows users to withdraw their balances. This state is typically active before a competition begins and after it has concluded.
2. **Locked**: When the escrow is locked, funds are secured and cannot be withdrawn. This state is active during the competition, ensuring that all necessary funds are held securely until the competition is complete.

Please note the following important considerations:

* Preset distributions cannot be changed once the escrow is locked, ensuring the integrity and immutability of the distribution rules.
* Funds cannot be withdrawn when the escrow is in a locked state, protecting the participants' contributions and the competition's prize pool.

The Arena DAO escrow system is designed to provide a secure, transparent, and flexible solution for managing funds in decentralized competitions, fostering trust and fairness among all participants.

---
description: Ensuring Fair and Transparent Fund Management
---

# Escrow

The escrow system is a cornerstone of Arena DAO's competition platform, ensuring fair and transparent management of funds and assets. Working in conjunction with the [Payment Registry](payment-registry.md), it provides a secure and reliable way to handle participant contributions, prize distributions, and withdrawals.

### Funding

* **Multi-Token Support**: Handles multiple token types, including:
  * CW20 tokens (fungible tokens)
  * Native tokens (e.g., ATOM, OSMO)
  * CW721 tokens (non-fungible tokens, or NFTs)
* **Locking Mechanism**: Secures funds once the competition is fully funded.
* **Withdrawal**: Allows fund withdrawal when in an unlocked state.

### Fund Distribution

* **Member-Percentage Distribution**: Allocates funds based on predefined percentages.
* **Remainder Address**: Receives leftover funds and all NFTs.

### Escrow States

1. **Unlocked**: Ready to receive funds and allow withdrawals.
2. **Locked**: Funds secured during the competition.

### Workflow

1. **Competition Setup**
   * Organizers create the competition and set parameters.
   * Participants register and set their distribution preferences in the Payment Registry.
2. **Funding Phase**
   * Escrow is in the Unlocked state.
   * Participants send required contributions to the escrow.
   * Once fully funded, the escrow transitions to the Locked state.
   * The competition's activation height is recorded.
3. **Competition Active**
   * Escrow remains in the Locked state.
   * Payment Registry records are immutable for this competition.
4. **Competition Conclusion**
   * Arena Core determines the winners and prize allocations.
5. **Distribution Process**
   * Arena Core queries the Payment Registry for each winner's distribution preferences.
   * The query uses the winner's address and the recorded activation height.
   * Escrow system processes distributions based on: a. Competition-level allocations (e.g., 1st place, 2nd place) b. Individual winner's Payment Registry preferences
6. **Withdrawal Phase**
   * Escrow transitions back to the Unlocked state.
   * Winners (individuals or teams) can withdraw their allocated funds.
   * For team distributions:
     * Funds are automatically subdivided according to the Payment Registry records.
     * Team members can withdraw their individual allocations directly.

# Augmented Bonding Curve

An Augmented Bonding Curve (ABC) is an advanced financial mechanism used in decentralized finance (DeFi) to create and manage sustainable token economies. It builds upon traditional bonding curves, incorporating additional features to ensure a more robust and balanced ecosystem.

For a deep dive into ABCs, check out these resources:

* [Deep Dive: Augmented Bonding Curves](https://medium.com/commonsstack/deep-dive-augmented-bonding-curves-b5ca4fad4436)
* [Continuous Organizations](https://medium.com/hackernoon/introducing-continuous-organizations-22ad9d1f63b7)

The implementation can be found [here](https://github.com/DA0-DA0/dao-contracts/pull/697).

> **Note:** The tokenomics described below are subject to change before the official launch of the Arena token. Please refer to our official communications for the most up-to-date information.

### Arena DAO's Transition to ABC

#### Initial Phase: Membership-Based DAO

Arena DAO will start as a membership-based organization, focusing on building a strong community foundation and establishing decentralized governance frameworks.

#### Transition: Token-Based Model

As we grow, we'll transition to a token-based model using the ABC, which will automate token supply management and align incentives between the DAO and early contributors.

### ABC Configuration for Arena DAO

* **Token:** ARENA
* **Total Supply:** 100,000,000 tokens
* **Pricing Model:** Square-root curve with USDC

#### Token Distribution

* Founder: 21,544,347 tokens (21.54%)
* Arena Gladiators: 10,335,410 tokens (10.34%)
* Reserved Liquidity: 2,319,762 tokens (2.32%)
* DAO Treasury: 20,088,833 tokens (20.09%)
* Open Phase Mint: 45,711,648 tokens (45.71%)

### Phases of the ABC

#### 1. Hatch Phase

* **Total Allocation:** 54,288,352 tokens (54.29% of total supply)
* **Participants:** Founder, Arena Gladiators, Community Pool
* **Exclusivity:** Only approved contributors can participate
* **Key Features:**
  * Initial token distribution to core team and early supporters
  * Establishes the foundation for the DAO's token economy
  * No public trading or liquidity at this stage

#### 2. Open Phase

* **Available for Minting:** 45,711,648 tokens (45.71% of total supply)
* **Entry Fee:** 99.999% (directly funds DAO treasury)
* **Exit Fee:** None
* **Key Features:**
  * Public participation begins
  * Continuous token minting based on the bonding curve
  * Dynamic pricing determined by token supply
  * AMM Liquidity Establishment:
    * Triggered after raising 10,000 USDC through minting
    * Creates a liquid market for ARENA tokens
    * Enables token swaps and improves price discovery

#### 3. Closed Phase (Future Consideration)

* **Purpose:** Potential mechanism for graceful shutdown or transition
* **Key Features:**
  * Allows only selling of tokens into the curve
  * No new minting permitted
  * Potential complete liquidation mechanism (not currently on roadmap)

### ABC Visualized

{% embed url="https://docs.google.com/spreadsheets/d/1UihzlAW_EgawsUIFcXlEUOCqGOwHfhVXwD-sIAUy7_s/edit?usp=sharing" fullWidth="true" %}
Charts on right side
{% endembed %}

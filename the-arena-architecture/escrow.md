# Escrow

The escrow system is a cornerstone of Arena DAO's competition platform, ensuring fair and transparent management of funds and assets.

### Key Functions

#### 1. Funding

* **Token Support**: The escrow handles multiple token types:
  * CW20 tokens
  * Native tokens
  * CW721 (NFT) tokens
* **Locking Mechanism**: Participants must send their dues to the escrow, locking them once completely funded for the duration of the competition.
* **Withdrawal**: Users can withdraw funds when the escrow is unlocked.

#### 2. Fund Distribution

The escrow employs a flexible distribution system to accommodate various competition structures:

**a. Member-Percentage Distribution**

* Funds are allocated based on a predefined member-percentage list.
* The sum of all percentages must equal 100%.

**b. Remainder Address**

* A designated address receives any leftover funds after member share calculations.
* All NFTs (CW721 tokens) are sent to the remainder address due to their indivisible nature.

**c. Preset Distributions**

* Members can establish preset distribution rules for incoming funds.
* Example: A DAO can specify an even distribution among its members, streamlining the process.
* Note: Preset distributions cannot be modified when the escrow is locked.

#### 3. Withdrawal Process

* After fund distribution, users can withdraw their new balances from the escrow.
* The withdrawal process is initiated by the user and executed by the smart contract.

### Escrow States

The escrow has two primary states:

1. **Unlocked**: Ready to receive funds and allow withdrawals.
2. **Locked**: Funds are secured during the competition.

Important notes:

* Preset distributions cannot be changed once the escrow is locked.
* Funds cannot be withdrawn when the escrow is in a locked state.

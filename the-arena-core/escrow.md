# Escrow

In the Arena DAO, the escrow plays a crucial role in competitions. Its main function is to ensure that the funds or assets contributed by the participants or hosts are protected and distributed in a fair and transparent manner according to the result of the competition.

### Funding:

At the start of a competition, participants are required to send their dues to the escrow to lock it. The escrow is designed to handle most types of tokens: CW20, native, and CW721. Users can withdraw funds whenever the escrow is unlocked.

{% hint style="info" %}
For more information on the escrow state, view the link below for a visual explanation!\
[competitions](competitions/ "mention")
{% endhint %}

### &#x20;Fund Distribution:

1. **Member-Percentage:** Escrow funds are distributed according to a member-percentage list. The sum of percentages must always equal 100%.&#x20;
2. **Remainder Address:** The remainder address is a designated address that receives any leftover funds after member shares are calculated. NFT's will always be sent to the remainder address, because they are not divisible into percentages.
3. **Preset Distributions:** Members can set preset distributions to flow incoming funds to other members. For example, a DAO can specify an even distribution to its members to avoid a lengthy proposal process. The preset distribution cannot be updated when the escrow is locked.

### Withdrawal:

After the distribution of funds is processed, users can withdraw their new balances from the escrow.&#x20;

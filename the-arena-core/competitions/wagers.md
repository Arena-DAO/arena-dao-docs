# Wagers

The Wager Module represents the most basic implementation of a competition module within the Arena ecosystem. It enables the creation and management of decentralized wagers.

### Wager Details

**Host:** The host of the competition is responsible for processing the results. In the Arena, this is defaulted to an automatically-generated DAO of the wager's members, requiring all members for consensus. However, there is also the option to designate a host, such as a referee or an existing DAO.

**Name:** Start by giving your wager a unique name. This helps participants and spectators identify your competition.&#x20;

**Description:** Provides a more in-depth overview of the competition.

**Expiration:** Decide when your wager will end. If the competition is not processed by then, the competition can be jailed where it can only be resolved by the Arena DAO. You have three options:&#x20;

* **At Time**
* **At Height** (block height)
* **Never**

**Rules:** Establish the rules that you consider fair and necessary for the competition. This includes how a winner is determined, specific restrictions, and any other guidelines that guide the competition fairly.

**Rulesets:** If the category of the competition has rulesets, feel free to apply these to streamline the rules setup.

**Dues:** Define the stakes of the wager and where funding is coming from. See more about dues in [escrow.md](../escrow.md "mention").

{% hint style="info" %}
For more information on the competition state, view the link below for a visual explanation!\
[.](./ "mention")
{% endhint %}

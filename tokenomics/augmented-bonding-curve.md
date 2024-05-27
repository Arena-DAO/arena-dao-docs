# Augmented Bonding Curve

An Augmented Bonding Curve (ABC) is an advanced financial instrument used in decentralized finance (DeFi) to facilitate the creation and management of token economies. It combines the principles of bonding curves with additional mechanisms to ensure more robust and sustainable ecosystems. Our implementation can be found [here](https://github.com/your-repo/cw-abc).

### Inspiration

* [Deep Dive: Augmented Bonding Curves](https://medium.com/commonsstack/deep-dive-augmented-bonding-curves-b5ca4fad4436)
* [Continuous Organizations](https://medium.com/hackernoon/introducing-continuous-organizations-22ad9d1f63b7)

### Transition from Membership to Token-Based DAO

Initially, the Arena DAO will operate as a membership-based organization focusing on building a strong community foundation and setting the groundwork for our decentralized governance. As we grow, the DAO will transition into a token-based model using the ABC. This transition will allow the DAO to automate token supply management effectively and align incentives between the DAO and its early contributors. Only [contributors](../introduction/contributor-guideline.md) will be allowed to participate in the hatch phase.

### ABC Configuration

* **Token Supply:** The ARENA token will have a capped supply of **100 million tokens**, governed by a square-root curve with **USDC**.
* **External Liquidity:** External liquidity will be set up as soon as the hatch phase ends.
* **Liquidity Mining Incentives:** $100k of the ABC funding will be allocated to provide liquidity mining incentives for the USD-ARENA pool.

#### Hatch Phase

In the hatch phase, early contributors (hatchers) can buy tokens with minimal friction, each having a limit according to their hatch configuration. This phase aims to bootstrap the DAO’s initial funding and token distribution.

* **Funding Goal:** Ends after raising 7k USDC (subject to change).
* **Founder Purchase:** The founder will buy first with a limit of 5k USDC.
* **Contributor Participation:** Contributors can then buy within their limits.

#### Open Phase

In the open phase, anyone can mint new tokens or sell them into the curve. The AMM pool and ABC will work together to create a dynamic and efficient market for ARENA tokens.

* An **entry fee** of **95%** will be applied to directly fund the DAO's treasury
* No exit fee will be applied

#### Closed Phase

In the closed phase, users can only sell tokens into the curve without friction. While not currently on the roadmap, this phase can serve as a complete liquidation mechanism for the token through the ABC if needed.

### ABC Visualized

{% embed url="https://docs.google.com/spreadsheets/d/192D4nuhlSwULwc7p3gPJlR4yB-SuGFShMziEPF9b8Sw/edit?usp=sharing" %}
Augmented Bonding Curve Visualized
{% endembed %}

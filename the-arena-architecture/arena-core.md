# Arena Core

The Arena Core is the central component of our architecture, storing and managing information critical to all competitions within the Arena DAO ecosystem. It serves as the backbone for our decentralized competition platform, ensuring consistency, fairness, and efficiency across all activities.

{% hint style="info" %}
Please note that the smart contracts used in this project have **not been audited**. While every effort has been made to ensure the security and accuracy of the code, we strongly advise conducting your own thorough review and due diligence before interacting with these contracts.
{% endhint %}

### Integration with DAO Pre-Propose Module

The Arena Core is built as an extension of a 'DAO pre-propose module', which allows for a streamlined dispute resolution process. This design enables the specific proposal of jailing competitions on the DAO, ensuring community-driven conflict resolution.

The proposal module is configured for revoting, meaning that jailed competitions will be resolved by a majority vote after a predetermined period. This approach guarantees fair and transparent dispute resolution, with the community having the final say on the outcome of disputed competitions.

### Key Components of the Arena Core

#### 1. Category Management

* Defines and manages distinct competition categories, ensuring a clear structure and organization within the platform
* Links categories to specific rulesets and rating systems, maintaining consistency and fairness across competitions

#### 2. Competition Jailing Mechanism

* Allows for the proposal of jailing competitions that are in dispute, preventing the continuation of controversial competitions until resolved
* Ensures community-driven dispute resolution through majority voting, giving the power to the community to decide on the outcome of disputed competitions

#### 3. Competitor Rating System

* Tracks and manages competitor rankings per category, providing a clear and transparent system for assessing participant performance
* Implements the Glicko-2 algorithm for fair and accurate rating calculations, ensuring that rankings reflect the true skill level of competitors

#### 4. Rulesets Repository

* Stores standardized rulesets per category, ensuring that all competitions within a category follow the same set of rules
* Allows for the creation and modification of custom rulesets, providing flexibility for unique competition formats
* Ensures consistency in rule application within each category, maintaining fairness and predictability for participants

#### 5. Competition Modules

* Modular components for creating diverse competition formats, allowing for a wide range of competition types and structures
* Enables easy creation and integration of new competition formats, fostering innovation and creativity within the platform

#### 6. Tax Rate Management

* Manages the platform's fee structure to sustain the ecosystem and support ongoing development and maintenance
* The tax rate at launch will be set at 5% of competition entry fees and prizes
* The tax rate can be updated through the DAO governance process, ensuring that the community has a say in the financial aspects of the platform

The Arena Core is designed to be robust, flexible, and community-driven, providing a solid foundation for the Arena DAO ecosystem to grow and thrive.

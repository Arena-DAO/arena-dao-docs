# Arena Core

The Arena Core is the central component of our architecture, storing and managing information critical to all competitions within the Arena DAO ecosystem. It serves as the backbone for our decentralized competition platform, ensuring consistency, fairness, and efficiency across all activities.

Importantly, the Arena Core is built as an extension of a 'DAO pre-propose module'. This design allows us to specifically propose jailing competitions on the DAO, streamlining the dispute resolution process. The proposal module is configured for revoting, meaning that jailed competitions will be resolved by a majority vote after a predetermined period of time, ensuring fair and community-driven conflict resolution.

Key components of the Arena Core include:

#### 1. Category Management

* Defines and manages distinct competition categories
* Links categories to specific rulesets and rating systems

#### 2. Competition Jailing Mechanism

* Allows for the proposal of jailing competitions in dispute
* Ensures community-driven dispute resolution through majority voting

#### 3. Competitor Rating System

* Tracks and manages competitor rankings per category
* Implements the Glicko-2 algorithm for fair and accurate rating calculations

#### 4. Rulesets Repository

* Stores standardized rulesets per category
* Allows for creation and modification of custom rulesets
* Ensures consistency in rule application within each category

#### 5. Competition Modules

* Modular components for creating diverse competition formats
* Allows for easy creation and integration of new competition formats

#### 6. Tax Rate Management

* Manages the platform's fee to sustain the ecosystem
* The tax rate at launch will be 5%
* Updated through the DAO

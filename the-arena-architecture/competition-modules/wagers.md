# Wagers

The Wager Module is the most basic implementation of a competition module within the Arena ecosystem. It enables users to create and manage decentralized wagers in a transparent and fair manner.

### Key Components

#### 1. Host

* **Default Setting**: An automatically-generated DAO of the wager's members, requiring consensus from all members.
* **Alternative Option**: Designation of a specific host, such as a referee or an existing DAO.
* **Responsibility**: Processing the results of the wager.

#### 2. Wager Configuration

**a. Name**

* A unique identifier for the wager.
* Helps participants and spectators easily recognize the competition.

**b. Description**

* Provides a detailed overview of the wager.
* Can include context, objectives, or any other relevant information.

**c. Banner**

* Allows users to specify an image to display for the competition.
* Enhances visual appeal and recognition of the wager.

**d. Expiration** Defines when the wager will end. Options include:

* **At Time**: Specific date and time.
* **At Height**: Specific blockchain block height.
* **Never**: No expiration set.

Note: If the competition is not processed by the expiration time, it can be "jailed" and resolved only by the Arena DAO.

**e. Rules**

* Establish fair and necessary guidelines for the competition.
* Include criteria for determining the winner, specific restrictions, and other relevant guidelines.

**f. Rulesets**

* If the wager's category has predefined rulesets, they can be applied to streamline the rules setup.

**g. Dues**

* Define the stakes of the wager.
* Specify the source of funding.
* For more detailed information about dues, refer to the Escrow page.

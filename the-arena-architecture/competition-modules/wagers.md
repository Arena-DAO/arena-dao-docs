# Wagers

The Wager Module is a specific implementation of a competition module within the Arena ecosystem. It enables users to create and manage decentralized wagers in a transparent, fair, and engaging manner.

## Key Components

### 1. Wager Management

#### a. Host

* **Options**:
  * Assign a specific referee (individual account).
  * Designate a pre-created DAO (e.g., a referee DAO).
* **Role**: Processes and finalizes the results of the wager.

#### b. Configuration

* **Name**: Unique identifier for the wager.
* **Description**: Comprehensive overview of the wager.
* **Banner**: Optional image representation.
* **Expiration**: Defines the end point (time, block height, or never).
  * Note: If not processed by expiration, the wager can be "jailed" and resolved only by the Arena DAO.
* **Rules**: Guidelines governing the wager.
* **Rulesets**: Pre-defined sets of rules that can be applied if available for the wager's category.

### 2. Financial Management

#### Dues

* Define stakes for the wager.
* Specify funding sources and amounts.
* For detailed information about dues handling, refer to the [Escrow page](../escrow.md).

#### 3. Stat Tracking

* **Performance Metrics**: Track key indicators for participants (e.g., win/loss ratio, total wagers won).
* **Achievements**: Award recognitions for outstanding performances or milestones.
* **Data Visualization**: Present stats in easily digestible formats (graphs, charts).

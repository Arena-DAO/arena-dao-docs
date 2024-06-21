# Leagues

## Arena League Module

The Arena League Module is an advanced implementation of a competition module within the Arena ecosystem. It builds upon the concepts of the Wager Module to enable the creation and management of round-robin style tournaments.

### Key Components

#### 1. Host

* Designated entity responsible for inputting match results and managing the tournament.
* Can be an individual, a referee, or an existing DAO.

#### 2. League Configuration

**a. Name**

* A unique identifier for the league.
* Helps participants and spectators easily recognize the competition.

**b. Description**

* Provides a detailed overview of the league.
* Can include context, objectives, or any other relevant information.

**c. Banner**

* Allows organizers to specify an image to display for the league.
* Enhances visual appeal and recognition of the tournament.

**d. Expiration** Defines when the league will end. Options include:

* **At Time**: Specific date and time.
* **At Height**: Specific blockchain block height.
* **Never**: No expiration set.

Note: If the competition is not processed by the expiration time, it can be "jailed" and resolved only by the Arena DAO.

**e. Rules**

* Establish fair and necessary guidelines for the league.
* Include criteria for determining winners, specific restrictions, and other relevant guidelines.

**f. Rulesets**

* If the league's category has predefined rulesets, they can be applied to streamline the rules setup.

**g. Dues**

* Define the stakes of the league.
* Specify the source of funding.

#### 3. League-Specific Parameters

**a. Teams**

* List of participating teams or individuals in the league.

**b. Points System**

* **Match Win Points**: Points awarded for winning a match.
* **Match Draw Points**: Points awarded for a draw.
* **Match Lose Points**: Points awarded for losing a match.

**c. Distribution**

* Defines how the prize pool will be distributed among final placements.

### How It Works

#### 1. Tournament Setup

* Organizers define standard competition details, list of participants, final distribution, and points system.
* The module automatically generate rounds with matches to ensure all participants play each other once.

#### 2. Match Management

* As each match concludes, the host inputs results into the system.
* A leaderboard is dynamically updated according to the league's configuration.

#### 3. Point Adjustments

* The host has the ability to adjust points to penalize or reward teams outside of match results.

#### 4. End of Tournament Processing

* When all matches are completed, the module calculates final standings.
* Prize funds are automatically distributed based on the predefined distribution.
* The algorithm efficiently handles placement ties to ensure fair distribution.

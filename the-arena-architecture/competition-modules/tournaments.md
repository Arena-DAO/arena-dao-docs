# Tournaments

## Arena Tournament Module

The Arena Tournament Module is an advanced implementation of a competition module within the Arena ecosystem. It enables the creation and management of elimination-style tournaments, offering both single and double elimination formats.

### Key Components

#### 1. Host

* Designated entity responsible for inputting match results and managing the tournament.
* Can be an individual, a referee, or an existing DAO.

#### 2. Tournament Configuration

**a. Name**

* A unique identifier for the tournament.
* Helps participants and spectators easily recognize the competition.

**b. Description**

* Provides a detailed overview of the tournament.
* Can include context, objectives, or any other relevant information.

**c. Banner**

* Allows organizers to specify an image to display for the tournament.
* Enhances visual appeal and recognition of the event.

**d. Expiration** Defines when the tournament will end. Options include:

* **At Time**: Specific date and time.
* **At Height**: Specific blockchain block height.
* **Never**: No expiration set.

Note: If the competition is not processed by the expiration time, it can be "jailed" and resolved only by the Arena DAO.

**e. Rules**

* Establish fair and necessary guidelines for the tournament.
* Include criteria for determining winners, specific restrictions, and other relevant guidelines.

**f. Rulesets**

* If the tournament's category has predefined rulesets, they can be applied to streamline the rules setup.

**g. Dues**

* Define the stakes of the tournament.
* Specify the source of funding.

#### 3. Tournament-Specific Parameters

**a. Elimination Type** Choose from the following options:

* Single Elimination without Third Place Match
* Single Elimination with Third Place Match
* Double Elimination

**b. Teams**

* List of participating teams or individuals in the tournament, ordered by seeding.

**c. Distribution**

* Defines how the prize pool will be distributed among final placements.

### How It Works

#### 1. Tournament Setup

* Organizers define standard competition details, list of seeded participants, elimination type, and prize distribution.
* The module automatically generate the tournament bracket based on the chosen elimination type and number of participants.

#### 2. Bracket Generation

* An optimal algorithm is used to create the tournament bracket.
* The algorithm gives preference to higher-seeded teams, ensuring a fair and competitive structure.

#### 3. Match Management

* As each match concludes, the host inputs results into the system.
* The bracket is dynamically updated, and the next round of matches is automatically determined.

#### 4. Tournament Progression

* Single Elimination: Losers are eliminated, winners progress to the next round.
* Double Elimination: Losers move to a "losers' bracket" for a second chance, winners continue in the "winners' bracket". A rebuttal match will be played if the loser's bracket winner beats the winners' bracket winner.

#### 5. End of Tournament Processing

* When all matches are completed, the module determines the final placements.
* Prize funds are automatically distributed based on the predefined distribution.

# Leagues

The Arena League Module is an advanced implementation of a competition module within the Arena ecosystem. It builds upon the concepts of the Wager Module to enable the creation and management of round-robin style tournaments.

## Key Components

### 1. League Management

#### a. Host

* **Options**:
  * Assign a specific referee (individual account).
  * Designate a pre-created DAO (e.g., a referee DAO).
* **Role**: Manages the league, inputs match results, and oversees the tournament progression.

#### b. Configuration

* **Name**: Unique identifier for the league.
* **Description**: Comprehensive overview of the league.
* **Banner**: Optional image representation.
* **Expiration**: Defines the end point (time, block height, or never).
  * Note: If not processed by expiration, the league can be "jailed" and resolved only by the Arena DAO.
* **Rules**: Guidelines governing the league.
* **Rulesets**: Pre-defined sets of rules that can be applied if available for the league's category.

### 2. Financial Management

Dues

* Define stakes or entry fees for the league.
* Specify funding sources and amounts.
* For detailed information about dues handling, refer to the Escrow page.

### 3. League-Specific Parameters

#### a. Teams

* List of participating teams or individuals in the league.

#### b. Points System

* **Match Win Points**: Points awarded for winning a match.
* **Match Draw Points**: Points awarded for a draw.
* **Match Lose Points**: Points awarded for losing a match.

#### c. Distribution

* Defines how the prize pool will be distributed among final placements.

#### 4. Stat Tracking

* **Performance Metrics**: Track key indicators for participants (e.g., wins, losses, draws, total points).
* **Leaderboards**: Real-time rankings based on points and other criteria.
* **Tiebreaker Mechanism**: Utilize tracked stats to resolve ties in final standings.
* **Achievements**: Award recognitions for outstanding performances or milestones.
* **Data Visualization**: Present stats in easily digestible formats (graphs, charts).

## How It Works

1. **Tournament Setup**
   * Organizers define standard competition details, list of participants, final distribution, and points system.
   * The module automatically generates rounds with matches to ensure all participants play each other once.
2. **Match Management**
   * As each match concludes, the host inputs results into the system.
   * The leaderboard is dynamically updated according to the league's configuration.
3. **Point Adjustments**
   * The host has the ability to adjust points to penalize or reward teams outside of match results.
4. **End of Tournament Processing**
   * When all matches are completed, the module calculates final standings.
   * Prize funds are automatically distributed based on the predefined distribution.
   * The algorithm efficiently handles placement ties to ensure fair distribution.

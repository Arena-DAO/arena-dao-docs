# Payment Registry

The Arena Payment Registry is designed to streamline and automate the distribution of competition rewards. This smart contract allows participants to predefine how their potential winnings should be allocated, enabling efficient and transparent payouts without requiring additional actions after a competition concludes.

### How It Works

1. **Integration with Arena Core**: The Payment Registry is queried by the competition modules during competition distributions.
2. **User-Defined Distributions**: Participants can set their desired distribution patterns before a competition is fully-funded (activated).
3. **Immutable Records**: The distribution is locked in at the competition's activation block height.
4. **Automatic Payouts**: When rewards are distributed, they are automatically subdivided according to the predefined allocations.

### Key Features

#### 1. Flexible Distribution Setting

Users can define complex distribution patterns to suit their needs. For example, a team could set up a distribution where:

* 50% goes to the team captain
* 30% is split equally among other team members
* 20% goes to the team's charity fund

#### 2. Immutability for Fairness

Once a competition is activated, the distribution set in the registry becomes immutable for that specific competition. This ensures that participants cannot change the payout structure after seeing the competition results, maintaining fairness and preventing disputes.

#### 3. Efficient Querying

The registry is designed for efficient querying, allowing the Arena Core to quickly retrieve distribution information for multiple participants when processing competition rewards.

### Use Cases

#### Team Payouts

A gaming team participating in an Arena tournament can predefine how their winnings should be split among team members, coaches, and the organization. This eliminates the need for manual calculations and transfers after each competition.

#### Affiliate Programs

Influencers or affiliates can set up distributions where a percentage of their winnings automatically goes to their followers or community members who supported their participation.

#### Charity Contributions

Participants can allocate a portion of their potential winnings to charitable causes, automating their contributions and increasing transparency.

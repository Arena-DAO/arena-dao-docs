# Leagues

The league module expands upon the concepts in the wager module to enable the creation of round-robin style tournaments.

### **How It Works**

* **Tournament Setup**: Organizers define the standard competition details with a list of participants, final distribution, and a points system. The smart contracts will automatically generate rounds with matches to ensure all members play each other once.
* **Match Management**: As each match concludes, the host will be inputting match results into the system to slowly build out a leaderboard according to the league's configuration. Only the Arena DAO can override match results.
* **Point Adjustments:** The Arena DAO also allows for point adjustments to penalize or reward any teams apart from the matches.
* **End of Tournament Processing**: When all matches are completed, the module calculates the final standings and automatically distributes the prize funds. Placement ties are efficiently handled by the algorithm to ensure a fair distribution.

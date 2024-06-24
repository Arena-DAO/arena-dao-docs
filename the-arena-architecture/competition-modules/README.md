# Competition Modules

Arena DAO offers a diverse range of competition modules, each designed to cater to different types of contests and user preferences. Our modular approach allows for flexible, scalable, and customizable competition experiences within the decentralized ecosystem.

```mermaid
flowchart TB
    Start([Start]) --> HasDues{Competition<br>Has Dues?}
    HasDues -->|Yes| ShouldActivateDues{Should Activate<br>On Funded?}
    HasDues -->|No| ShouldActivateNoDues{Should Activate<br>On Funded?}
    
    ShouldActivateDues -->|Yes| PendingDues[Pending:<br>Awaiting Dues]
    ShouldActivateDues -->|No| PendingManual[Pending:<br>Manual Activation]
    
    ShouldActivateNoDues -->|Yes| ActiveCompetition[Active Competition]
    ShouldActivateNoDues -->|No| PendingManual
    
    PendingDues -->|All Dues Paid| ActiveCompetition
    PendingManual -->|Host Manually<br>Activates| ActiveCompetition
    
    ActiveCompetition -->|Expiration Reached| ConsensusCheck{Consensus<br>Reached?}
    ConsensusCheck -->|Yes| InactiveCompetition[Inactive Competition]
    ConsensusCheck -->|No| JailedCompetition[Jailed Competition]
    
    JailedCompetition -->|Arena DAO<br>Resolves| InactiveCompetition
    
    InactiveCompetition --> End([End])
    
    UnlockedEscrow[Escrow:<br>Unlocked] -->|Competition<br>Activated| LockedEscrow[Escrow:<br>Locked]
    LockedEscrow -->|Competition<br>Resolved| UnlockedEscrow
    
    PendingDues -.-> UnlockedEscrow
    PendingManual -.-> UnlockedEscrow
    ActiveCompetition -.-> LockedEscrow
    InactiveCompetition -.-> UnlockedEscrow
    
    classDef default fill:#4EA5D9,stroke:#2E4057,stroke-width:2px,color:#2E4057;
    classDef decision fill:#F99B45,stroke:#2E4057,stroke-width:2px,color:#2E4057;
    classDef escrow fill:#73D2DE,stroke:#2E4057,stroke-width:2px,color:#2E4057;
    classDef startend fill:#2ECC71,stroke:#2E4057,stroke-width:2px,color:#2E4057;
    
    class HasDues,ShouldActivateDues,ShouldActivateNoDues,ConsensusCheck decision;
    class UnlockedEscrow,LockedEscrow escrow;
    class Start,End startend;

```

### Available Modules

{% content-ref url="wagers.md" %}
[wagers.md](wagers.md)
{% endcontent-ref %}

{% content-ref url="leagues.md" %}
[leagues.md](leagues.md)
{% endcontent-ref %}

{% content-ref url="tournaments.md" %}
[tournaments.md](tournaments.md)
{% endcontent-ref %}

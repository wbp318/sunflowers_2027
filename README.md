# Sunflowers 2027 — Processing Feasibility Research

Research outline for starting sunflower processing in East Carroll Parish, Louisiana and the surrounding Delta (northeast LA, southeast AR, west MS).

Sunflowers grow well here, but there is **no local processing or buyer** — this repo holds the research on what it would take to change that.

- **[REPORT.md](REPORT.md)** — the full fact-checked research report: processing pathways, market prices, nearest buyers and freight, elevator-partnership model, grants, and next steps.
- **[VISERION_PLAN.md](VISERION_PLAN.md)** — partnership proposal and full financial model for Viserion Grain's Lake Providence river elevator (fee schedule, P&L tiers, grower economics, sensitivity, go/no-go gates).
- **[deck/viserion_deck.html](deck/viserion_deck.html)** — slide deck for the Viserion pitch meeting.

## How the Viserion program works

```mermaid
flowchart TD
    subgraph LEGEND[Legend]
        direction LR
        LG1[Base-case flow — solid arrows]:::base --> LG2[Money outcome]:::money
        LG3[Option / future — dashed arrows]:::opt -.-> LG4{{Gate / precondition}}:::gate
    end

    GATES{{"GATES — all four before any commitment:
    1 · Signed offtake with Red River (Lubbock)
    2 · Real freight quotes (truck spot + barge)
    3 · Viserion insurance sign-off on dryer protocol
    4 · 2,000 acres of grower letters of intent"}}:::gate

    GATES -.->|all four cleared| PLANT

    PLANT[Plant pilot — Mar–Apr 2027<br/>~2,000 ac high-oleic, AOG contracts<br/>signed with buyer pre-plant]:::base
    PLANT -->|grow season<br/>oil premium: +2%/pt over 40% oil| H[Harvest Aug–early Sep<br/>1,600 lb/ac dryland · 2,200 irrigated<br/>ahead of the corn/soybean rush]:::base
    H -->|~64 grower truckloads<br/>within ~50 mi| REC

    subgraph V[Viserion Grain — Lake Providence river elevator]
        REC[Receive · weigh · grade<br/>fee $0.45/cwt]:::base --> DRY[Dry to 10% moisture<br/>7–8% for summer carry<br/>daily fines housekeeping = fire control<br/>fee $0.50/cwt]:::base
        DRY --> STO[Segregated bin ~100k bu<br/>identity-preserved high-oleic<br/>fee $0.30/cwt · 2 mo avg]:::base
        STO --> MER[Freight coordination desk<br/>fee $0.10/cwt<br/>total fees $1.35/cwt · contribution ~$0.80/cwt]:::base
    end

    MER -->|truck $3.60/cwt est.<br/>500 cwt/load · ~600 mi| LUB[Red River Commodities<br/>Lubbock, TX — birdseed<br/>BASE CASE · delivered ~$22.75/cwt]:::base
    MER -.->|barge ~$1.00/cwt<br/>river-elevator exclusive| GULF[Gulf / export buyer<br/>saves $2.60/cwt ≈ $42/ac<br/>if buyer found — gate 2]:::opt
    MER -.->|2029 · only if ≥5,000 ac<br/>and vendor quotes check out| JV[Cleaning + bagging JV<br/>regional birdseed & deer-plot seed<br/>$150–500k capital · no freight penalty]:::opt

    LUB --> OUT[Grower farmgate ≈ $17.80/cwt → +$35 to +$157/ac<br/>Viserion contribution $25.6k → $128k/yr at 2k → 10k ac]:::money
    GULF -.-> OUT
    JV -.-> SCALE[Scale decision — winter 2027:<br/>Structure B merchandising · more acres · barge lane]:::opt
    OUT --> SCALE

    classDef base fill:#f5e6c4,stroke:#b8841c,color:#20261f
    classDef opt fill:#dceee8,stroke:#0e8a6b,color:#20261f,stroke-dasharray:4 3
    classDef money fill:#0e8a6b,stroke:#0a6b53,color:#ffffff
    classDef gate fill:#fdf3f0,stroke:#b4452e,color:#20261f
```

Generated 2026-07-20 from a multi-source deep-research pass (22 sources fetched, 76 claims extracted, 25 adversarially verified: 20 confirmed, 5 refuted).

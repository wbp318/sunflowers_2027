# Sunflowers 2027 — Processing Feasibility Research

Research outline for starting sunflower processing in East Carroll Parish, Louisiana and the surrounding Delta (northeast LA, southeast AR, west MS).

Sunflowers grow well here, but there is **no local processing or buyer** — this repo holds the research on what it would take to change that.

- **[REPORT.md](REPORT.md)** — the full fact-checked research report: processing pathways, market prices, nearest buyers and freight, elevator-partnership model, grants, and next steps.
- **[VISERION_PLAN.md](VISERION_PLAN.md)** — partnership proposal and full financial model for Viserion Grain's Lake Providence river elevator (fee schedule, P&L tiers, grower economics, sensitivity, go/no-go gates).
- **[deck/viserion_deck.html](deck/viserion_deck.html)** — slide deck for the Viserion pitch meeting.

## How the Viserion program works

```mermaid
flowchart TD
    G[Delta growers<br/>~2,000 ac pilot, AOG contracts signed pre-plant] -->|harvest Aug–Sep| V

    subgraph V[Viserion Grain — Lake Providence elevator]
        R[Receive, weigh, grade<br/>$0.45/cwt] --> D[Dry to 10% moisture<br/>daily fines housekeeping<br/>$0.50/cwt]
        D --> S[Segregated bin storage<br/>identity-preserved high-oleic<br/>$0.30/cwt]
    end

    S -->|truck $3.60/cwt<br/>500 cwt/load| L[Red River Commodities<br/>Lubbock, TX — birdseed<br/>base case]
    S -.->|barge ~$1.00/cwt<br/>Viserion-only option| N[Gulf / export buyer<br/>worth ~$42/ac if found]
    S -.->|2029, if ≥5,000 ac| C[On-site cleaning + bagging JV<br/>regional birdseed & deer-plot seed<br/>no freight penalty]

    L --> P[Grower farmgate ≈ $17.80/cwt<br/>Viserion contribution ≈ $0.80/cwt]

    GATES{{Gates before commitment:<br/>1. signed offtake · 2. real freight quotes<br/>3. insurance sign-off · 4. 2,000 ac of LOIs}} -.-> G
```

Generated 2026-07-20 from a multi-source deep-research pass (22 sources fetched, 76 claims extracted, 25 adversarially verified: 20 confirmed, 5 refuted).

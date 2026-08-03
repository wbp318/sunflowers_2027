# Sunflowers 2027 — Processing Feasibility Research

Research outline for starting sunflower processing in East Carroll Parish, Louisiana and the surrounding Delta (northeast LA, southeast AR, west MS).

Sunflowers grow well here, but there is **no local processing or buyer** — this repo holds the research on what it would take to change that.

- **[REPORT.md](REPORT.md)** — the full fact-checked research report: processing pathways, market prices, nearest buyers and freight, elevator-partnership model, grants, and next steps.
- **[VISERION_PLAN.md](VISERION_PLAN.md)** — partnership proposal and full financial model for Viserion Grain's Lake Providence river elevator (fee schedule, P&L tiers, grower economics, sensitivity, go/no-go gates).
- **[deck/viserion_deck.html](deck/viserion_deck.html)** — slide deck for the Viserion pitch meeting.

## How the Viserion program works

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "fontSize": "18px",
    "fontFamily": "Segoe UI, Avenir, sans-serif",
    "textColor": "#20261f",
    "primaryColor": "#f5e6c4",
    "primaryBorderColor": "#b8841c",
    "primaryTextColor": "#20261f",
    "lineColor": "#7a8076",
    "clusterBkg": "#f7f4ea",
    "clusterBorder": "#b8841c",
    "edgeLabelBackground": "#f7f4ea"
  },
  "flowchart": { "useMaxWidth": false, "nodeSpacing": 55, "rankSpacing": 65, "curve": "basis" }
}}%%
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

    subgraph PRE[Phase 0 — Aug–Dec 2026 · Deal-making]
        B1[Call Red River Commodities Lubbock<br/>+ NSA buyer directory second outlets<br/>ask: delivered price · quality spec · volume cap]:::base
        B2[Freight quotes:<br/>truck spot Lake Providence→Lubbock<br/>barge Lake Providence→NOLA oilseed rate]:::base
        B3[Viserion working session:<br/>Structure A fee schedule · one segregated bin<br/>ops + insurer review of dryer fire protocol]:::base
        B4[Grower recruiting meetings:<br/>rotation ground · marginal dryland · irrigated acres<br/>target 2,000 ac of LOIs ≈ 64 loads minimum]:::base
        B5[USDA VAPG planning grant ~$75k<br/>funds professional feasibility study<br/>watch LDAF RFSI next round]:::opt
        B1 --> GATES
        B2 --> GATES
        B3 --> GATES
        B4 --> GATES
        B5 -.-> B3
    end

    GATES -.->|all four cleared → term sheet Dec 2026<br/>AOG contracts signed grower↔buyer Jan–Feb 2027| PLANT
    GATES -.->|any gate fails| KILL[STOP — no capital committed<br/>kill conditions: no offtake · truck >$4.25/cwt<br/>with no barge buyer · insurer balks · <2,000 ac]:::gate

    subgraph FARM[Phase 1 — 2027 crop year · Grower side]
        PLANT[Plant Mar–Apr 2027 · high-oleic varieties<br/>seed $30 + fert $70 + chem $55 + ops $45<br/>+ harvest $40 + ins $10 ≈ $250/ac dryland]:::base
        PLANT -->|"oil premium: +2% price per point >40% oil<br/>45% oil ⇒ +$2.28/cwt ⇒ +$36/ac free"| H[Harvest Aug–early Sep<br/>dryland 1,600 lb/ac = 16 cwt<br/>irrigated 2,000–2,200 lb/ac<br/>lands BEFORE corn/soybean rush]:::base
        H -->|combine at 12–15% moisture<br/>haul wet within ~50 mi| REC
    end

    subgraph V[Phase 2 — Viserion Lake Providence elevator — ex Zen-Noh/Bunge river terminal]
        REC[RECEIVE · weigh · grade · dock for FM<br/>fee $0.45/cwt<br/>uses existing pits + scales, slack season]:::base
        REC --> DRY[DRY to 10% moisture — 7–8% if summer carry<br/>avg 3 points removed · fee $0.50/cwt<br/>⚠ fines = fire risk: DAILY dryer cleanout<br/>NDSU: housekeeping, not temperature]:::base
        DRY --> STO[STORE segregated ~100k bu bin<br/>holds ~30,000 cwt at 28–32 lb/bu test weight<br/>identity-preserved · fee $0.15/cwt/mo × 2 mo = $0.30]:::base
        STO --> MER[MERCHANDISE / coordinate freight<br/>fee $0.10/cwt margin, freight at cost<br/>FEE STACK $1.35/cwt − var cost $0.55<br/>= CONTRIBUTION ~$0.80/cwt]:::base
    end

    MER -->|"truck: $1,800/load ÷ 500 cwt = $3.60/cwt<br/>weight-limited at 50,000 lb · 1 load ≈ 31 ac<br/>USDA S-Central rate extrapolated past 200 mi"| LUB[BASE CASE · Red River Commodities<br/>Lubbock TX birdseed/wildlife · ~600 mi<br/>delivered ~$22.75/cwt Oct-25 ref bid<br/>range seen 2021: $16.60→$31.40]:::base
    MER -.->|"barge: ~$0.75–1.00/cwt to Gulf<br/>saves ~$2.60/cwt vs truck ≈ $42/ac<br/>ONLY a river elevator can offer this"| GULF[OPTION · Gulf / export buyer<br/>NOLA transload · Mexico + EU birdseed demand<br/>needs buyer found — none identified yet]:::opt
    MER -.->|"2029 decision · needs ≥5,000 ac<br/>+ written vendor quotes — all internet<br/>equipment prices were refuted in verification"| JV[OPTION · Structure C bagging JV<br/>clean/screen/bag black-oil + deer-plot seed<br/>$150–500k capital placeholder<br/>sells regional: feed stores, co-ops, hunters<br/>zero freight penalty on every bag]:::opt

    LUB --> GN[GROWER NET · farmgate $17.80/cwt<br/>= $22.75 − $3.60 frt − $1.35 fees<br/>dryland +$35/ac · +oil premium +$71/ac<br/>irrigated+premium +$157/ac<br/>⚠ at $20 delivered: truck = −$9/ac]:::money
    LUB --> VN[VISERION NET · $0.80/cwt contribution<br/>2,000 ac → $25.6k · 5,000 ac → $64k<br/>10,000 ac → $128k/yr<br/>vs $25–75k one-time setup: payback 1–3 seasons<br/>+ Structure B adds $0.20–0.50/cwt basis margin]:::money
    GULF -.->|+$42/ac to growers| GN
    JV -.->|retail margin upside| VN

    GN --> SCALE{{Winter 2027 scale review:<br/>quality history? buyer performance?<br/>grower re-signs? → Structure B 2028:<br/>Viserion posts local bid, owns seed,<br/>arbitrages Lubbock vs barge vs crushers}}:::gate
    VN --> SCALE
    SCALE -.->|volume ≥5,000 ac| JV
    SCALE -.->|thin margins persist<br/>or buyer exits| KILL

    classDef base fill:#f5e6c4,stroke:#b8841c,color:#20261f
    classDef opt fill:#dceee8,stroke:#0e8a6b,color:#20261f,stroke-dasharray:4 3
    classDef money fill:#0e8a6b,stroke:#0a6b53,color:#ffffff
    classDef gate fill:#fdf3f0,stroke:#b4452e,color:#20261f
```

Generated 2026-07-20 from a multi-source deep-research pass (22 sources fetched, 76 claims extracted, 25 adversarially verified: 20 confirmed, 5 refuted).

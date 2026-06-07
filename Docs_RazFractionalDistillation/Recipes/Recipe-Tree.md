---
tags:
  - satisfactory
  - mod
  - recipes
  - distillation
title: Recipe Tree - Crude Oil Fractional Distillation
In Editor Class:
---

# Fractional Distillation

> [!INFO] Prepare for oil and oil derivatives
> The full production web for the mod, starting with the fractional distillation of oil.

> [!WARNING]- Power Changes and Local Maximums 
> Power Values are not final and are subject to rebalancing.
> Values listed on the diagram are highest throughput recipes, see Tower Focuses below for details

```mermaid
flowchart LR
    %% --- Raw input ---
    WELL[(Oil Well)] -->|Crude Oil: 120| FT{{Fractionating Tower}}

    %% --- Primary fractions, top of tower to bottom ---
    FT --> RG[Refinery Gas<br/>120]
    FT --> GAS[Gasoline<br/>80]
    FT --> KER[Kerosene<br/>60]
    FT --> DSL[Diesel<br/>45]
    FT --> RES[Heavy Residue<br/>45]

    %% --- Downstream chains ---
    RG --> PREF{{Plastic Refinery}} --> PLAS[Plastic: 40]
    GAS --> GGEN{{Gasoline Generator}} --> PWR1[Power ~150 MW]
    KER --> JET{{Jet Workshop}} --> JFUEL[Jet Fuel: 30]
    DSL --> DGEN{{Diesel Generator}} --> PWR2[Power ~250 MW]
    RES --> COKE{{Coker Unit}}
    COKE --> BIT[Bitumen: 20]
    COKE --> LUBE[Lubricant: 10]

	%% --- Helpful products ---
	LUBE --> ROTORS[Rotor Alt]
	BIT --> BONDEDPLATE[Reinforced Plate Alt]

    %% --- Styling ---
    style WELL fill:#3a2d1a,stroke:#e0a030,color:#fff
    style FT fill:#1a2a3a,stroke:#30a0e0,color:#fff
    classDef product fill:#1d3a1d,stroke:#40c040,color:#fff;
    class PLAS,JFUEL,BIT,LUBE,PWR1,PWR2 product;
```

> [!TIP]- Rotor Alternate Recipe
> Massively improved rotor production speed and greater efficiency.

> [!TIP]- Reinforced Plate Alternate Recipe
>Although using higher throughputs of iron, mixing with bags of bitumen increases the speed
>greatly, improving the output by four times whilst keeping the same iron to plate ratio.

---

| Fraction        | Tower height | Rate /min | Primary downstream | Final product   |
| --------------- | :----------: | --------: | ------------------ | --------------- |
| Refinery Gas    | Top          |       120 | Plastic Refinery   | Plastic         |
| Gasoline        | Upper        |        80 | Gasoline Generator | Power           |
| Kerosene        | Middle       |        60 | Jet Workshop       | Jet Fuel        |
| Diesel          | Lower        |        45 | Diesel Generator   | Power           |
| Heavy Residue   | Bottom       |        30 | Coker Unit         | Bitumen + Lube  |

---

# Heavy Residue with the Coker

```mermaid
flowchart TD
    RES[Heavy Residue: 30] --> COKE{{Coker Unit}}
    COKE -->|66%| BIT[Bitumen: 20]
    COKE -->|33%| LUBE[Lubricant: 10]
    BIT --> ASM{{Assembler}} --> PLATE[Reinforced Plate Alternate]
    LUBE --> ASM{{Assembler}} --> GEAR[Lubricated Rotor Alternate]
    classDef product fill:#1d3a1d,stroke:#40c040,color:#fff;
    class PLATE,GEAR product;
```

---

## Tower Focuses

> [!TIP] Temperature Ranges
> | Temp | Focus | Input | Outputs | Time |
> | ------------------------------- | ----------------------- | ------------- | ---------------------------------------------- | ---: |
> | Extreme Temp (~400 °C) | Heavy Residue / Bitumen | 30 Crude Oil  | Only 45 Residue   | 4 s |
> | High Temp (~350 °C)    | Diesel                  | 60 Crude Oil  | 45 Diesel No · Refinery Gas | 5 s |
> | Medium Temp (~250 °C)  | Kerosene                | 80 Crude Oil  | 60 Kerosene · No Residue               | 6 s |
> | Low Temp (~150 °C)     | Gasoline                | 100 Crude Oil | 80 Gasoline · 60 Refinery Gas              | 7 s |
> | Minimal Temp (~50 °C)  | Refinery Gas            | 120 Crude Oil | Only 120 Refinery Gas              | 8 s |

---

> [!SUCCESS] You should probably check out [Plastics](00-Plastic-Ladder.md)
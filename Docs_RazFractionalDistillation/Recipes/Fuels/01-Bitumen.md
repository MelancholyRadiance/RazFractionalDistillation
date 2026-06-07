---
tags:
  - satisfactory
  - mod
  - recipes
  - fuels
  - tier1
title: Bitumen - T1 Fuel
tier: 1
In Editor Class:
---

# 🛢️ Bitumen (T1)

> [!INFO] Tier 1 fuel
> The bottom of the barrel, literally.
>  The tarry residue left after distillation, bagged and burned as is.
 
---

## Main recipe - Residue Tapping

```mermaid
flowchart LR
    HR[Heavy Residue: 30] --> M{{Coker Unit}} --> BIT[Bitumen: 30]
```

| | Input | Output | Building | Time |
|---|---|---|---|---|
| **Main** | 30 Heavy Residue | 30 Bitumen | Coker Unit | 4 s |

---

## Alternate 1 - Crude Sludge

> [!WARNING] Low Yield, Burn unrefined crude straight into bitumen
> Bypassing the tower throws away the light fractions, this can simplify the production be rids of important chemicals.

| Input        | Output     | Building   | Time |
| ------------ | ---------- | ---------- | ---- |
| 40 Crude Oil | 20 Bitumen | Coker Unit | 6 s  |

---

## Alternate 2 - Residue Blending

> [!TIP] Manufacturing Bitumen can provide huge throughputs for massive burner arrays.

| Input                        | Output      | Building | Time |
| ---------------------------- | ----------- | -------- | ---- |
| 20 Heavy Residue + 10 Diesel | 120 Bitumen | Blender  | 6 s  |

---

> [!SUCCESS] Next tier: **[Petroleum Coke (T2)](./02-Petroleum-Coke.md)**

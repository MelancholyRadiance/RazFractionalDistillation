---
tags:
  - satisfactory
  - mod
  - recipes
  - rubber
  - tier1
title: Crude Rubber - T1
tier: 1
In Editor Class:
---

# ⚫ Crude Rubber (T1)

> [!INFO] Tier 1 rubber
> A cheap, tacky elastomer cooked from bitumen under heat. Weak and sticky, but
> it seals and cushions in a pinch.

---

## Main recipe - Bitumen Curing

```mermaid
flowchart LR
    BIT[Bitumen: 20] --> M{{Curing Oven}}
    M --> CR[Crude Rubber: 20]
```

|          | Input                | Output          | Building    | Time |
| -------- | -------------------- | --------------- | ----------- | ---- |
| **Main** | 20 Bitumen + 5 Water | 12 Crude Rubber | Curing Oven | 6 s  |

---

## Alternate 1 - Residue Curing

Use raw heavy residue instead of refined bitumen - cheaper, lower yield.

| Input            | Output         | Building    | Time |
| ---------------- | -------------- | ----------- | ---- |
| 30 Heavy Residue | 8 Crude Rubber | Curing Oven | 8 s  |

---

## Alternate 2 - Sulfur Bonus *(optional)*

Spend surplus sulfur from the fuel line for a higher yield - never required.

| Input | Output | Building | Time |
|---|---|---|---|
| 20 Bitumen + 10 Sulfur | 30 Crude Rubber | Curing Oven | 6 s |

---

> [!SUCCESS] Next tier: **[Synthetic Rubber (T2)](./02-Synthetic-Rubber.md)**

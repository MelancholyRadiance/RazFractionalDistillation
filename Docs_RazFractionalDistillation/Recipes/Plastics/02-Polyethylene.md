---
tags:
  - satisfactory
  - mod
  - recipes
  - plastics
  - tier2
title: Polyethylene - T2
tier: 2
In Editor Class:
---

# 🟪 Polyethylene (T2)

> [!INFO] Tier 2 plastic
> The workhorse plastic. Crack gas into ethylene, then polymerize it properly.
> Reliable, flexible, the backbone of mid-game manufacturing.

---

## Main recipe - Ethylene Polymerization

```mermaid
flowchart LR
    ETH[Ethylene: 30] --> M{{Polymerizer}} --> PE[Polyethylene: 30]
```

| | Input | Output | Building | Time |
|---|---|---|---|---|
| **Main** | 30 Ethylene | 30 Polyethylene | Polymerizer | 4 s |

---

## Alternate 1 - Integrated Cracking *(skip standalone ethylene)*

Crack and polymerize in one line straight from gas.

| Input | Output | Building | Time |
|---|---|---|---|
| 50 Refinery Gas + 10 Water | 30 Polyethylene | Polymerizer | 6 s |

---

## Alternate 2 - Crude Reforming

Re-process T1 crude plastic into proper polyethylene.

| Input | Output | Building | Time |
|---|---|---|---|
| 30 Crude Plastic + 10 Ethylene | 30 Polyethylene | Polymerizer | 6 s |

---

>[!TIP] Polyethylene Direct Uses
>Unlike "crude plastic" polyethylene is its own item, it allows better recipes for stators, modular frames and even computers
>but can also be turned into regular old plastic at a 1:1

---
> [!SUCCESS] Next tier: **[Polypropylene (T3)](./03-Polypropylene.md)**

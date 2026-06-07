---
tags:
  - satisfactory
  - mod
  - recipes
  - intermediates
title: Butadiene
In Editor Class:
---

# 🧪 Butadiene

> [!INFO] Monomer
> The C4 cracking product, feedstock for synthetic rubber.

---

## Main recipe - Gas Cracking

```mermaid
flowchart LR
    RG[Refinery Gas: 50] --> M{{Steam Cracker}}
    M --> BUTA[Butadiene: 20]
```

| | Input | Output | Building | Time |
|---|---|---|---|---|
| **Main** | 50 Refinery Gas | 20 Butadiene | Steam Cracker | 6 s |

---

## Alternate 1 - Ethylene Dimerization

Build butadiene up from surplus ethylene.

| Input       | Output       | Building | Time |
| ----------- | ------------ | -------- | ---- |
| 30 Ethylene | 20 Butadiene | Refinery | 6 s  |

---

## Alternate 2 - Gasoline Extraction

Pull butadiene from a cracked gasoline cut - higher yield, consumes fuel stock.

| Input | Output | Building | Time |
|---|---|---|---|
| 30 Gasoline | 30 Butadiene | Steam Cracker | 8 s |

---
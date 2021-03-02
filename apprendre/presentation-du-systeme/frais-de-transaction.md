---
description: En savoir plus sur les frais de transaction d'Avalanche
---

# Frais de transaction

Afin d'éviter le spam, les transactions sur Avalanche nécessitent le paiement de frais de transaction. Les frais sont payés en [AVAX](../../#avalanche-avax-jeton). **Les frais de transaction sont brûlés \(détruits à jamais\)**.

Lorsque vous effectuez une transaction via l'API d'Avalanche, les frais de transaction sont automatiquement déduits de l'une des adresses que vous contrôlez.

## Barème des frais

Différents types de transactions nécessitent le paiement de frais de transaction différents. Ce tableau présente le barème des frais de transaction :

```cpp
+----------+-------------------+------------------------+
| Chain    : Transaction Type  | Transaction Fee (AVAX) |
+----------+-------------------+------------------------+
| P        : Create Blockchain |                   0.01 |
+----------+-------------------+------------------------+
| P        : Add Validator     |                      0 |
+----------+-------------------+------------------------+
| P        : Add Delegator     |                      0 |
+----------+-------------------+------------------------+
| P        : Create Subnet     |                   0.01 |
+----------+-------------------+------------------------+
| P        : Import AVAX       |                  0.001 |
+----------+-------------------+------------------------+
| P        : Export AVAX       |                  0.001 |
+----------+-------------------+------------------------+
| X        : Send              |                  0.001 |
+----------+-------------------+------------------------+
| X        : Create Asset      |                   0.01 |
+----------+-------------------+------------------------+
| X        : Mint Asset        |                  0.001 |
+----------+-------------------+------------------------+
| X        : Import AVAX       |                  0.001 |
+----------+-------------------+------------------------+
| X        : Export AVAX       |                  0.001 |
+----------+-------------------+------------------------+
```

Le prix du gaz de la [C-Chain](./#chaine-de-contrat-c-chain) est de 4,7e-7 AVAX / gaz. La limite de gaz de la C-Chain est de 10e8.


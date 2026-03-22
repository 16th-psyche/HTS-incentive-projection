# 📊 QuantumLeap: System Rules & Calculation Parameters

This document outlines the strict mathematical parameters, threshold constraints, and system workflows natively embedded into your FY26-27 Incentive Projection Dashboard tool. 

---

## 1. Product Valuations
Four distinct product classes automatically merge into total collection yields globally.
Default internal configuration variables are as follows:
* **MBA Units**: `₹7,97,000`
* **BSA Units**: `₹2,46,000`
* **MBA Renewal (MBA-R)**: `₹5,00,000` 
* **BSA to MBA Renewal**: `₹6,15,000`

**Total Monthly Collection** = Sum of *(Unit Sold x Its Valuated Price)* across all four product bands for the specific timeframe.

---

## 2. Sales Rep Slabs & Payout Matrix
For a representative to unlock any incentive percentile yield, they must meet **strictly both** the *Minimum Unit Volume* and the *Minimum Cash Collection* constraints inside the exact same calendar month. Slabs are not aggregate across quarters.

* **Slab 1 (Cyan):** Minimum `3 Units` AND `₹17,97,000` Collection -> Yields **3.0%**
* **Slab 2 (Orange):** Minimum `4 Units` AND `₹22,000,000` Collection -> Yields **4.0%**
* **Slab 3 (Green):** Minimum `6 Units` AND `₹35,000,000` Collection -> Yields **5.0%**
* **Slab 4 (Gold):** Minimum `8 Units` AND `₹45,000,000` Collection -> Yields **6.0%**

*Note on Down-tiering:* If a representative hits 10 massive product units but generates only ₹15L in cash collection (missing the minimum ₹17.97L barrier), their threshold maps to `No Slab (0%)` structurally. Validations must cover BOTH metrics.

---

## 3. Dynamic Salary Engine (Chronological Routing)
Base salary disbursements in the tool are time-aware and react to drop-down markers configured in the `Team & Settings` tab. 

1. **Pre-Active Status:** Any month scheduled chronologically *before* a member's chosen "Active From" tag forces their recorded monthly salary to exactly **₹0** without affecting total unit accumulations.
2. **Active State:** Between their Start Date and Appraisal bounds, they continuously draw their strict standard "Salary".
3. **Appraisal Trigger:** Any month sequenced *on or after* the "Appraisal In" dropdown will aggressively strip their old base salary entirely from that month onward, dropping in their stated "Appraised Salary" block logically.

---

## 4. Manager Target Overrides
Managers are placed globally above generic tiers, subject to massive macro-targets. To unlock their direct payout override percentile, the **Overall System Aggregate Component** must clear global targets:

* **Trigger Condition:** The Combined Team performance must exceed `14 Total Units` **AND** `₹85,00,000 Total Collection` globally inside the same given month.
* **Payout Calculation:** When successful (labeled visually as `MET`), the Manager earns their highly specific target fraction boundary (`0.6%` or `0.4%`) of the **Total Team Aggregate Collection Balance**, paid directly alongside their active dynamic salary row constraints.

---

## 5. Global Metrics & State
* **Revenue Pool:** The total sum of every single sale enacted globally across FY26-27.
* **Total Expenses:** The complete numerical sum of all distributed `Base Salaries` (Reps + Managers) plus all `Incentive Yields` won.
* **Expense Percentage Calculation:** Mathematically mapped mathematically internally as:  
  `Expense % = (Total Expenses / Revenue Pool) * 100`  
  This updates in absolutely real-time directly inside the top status banner whenever any single field is modified.

*All system configurations, names, and slab overrides are cached permanently on the current device using the `localStorage API` (Namespace: `incentiveProjectionStateV2`). No databases are utilized.*

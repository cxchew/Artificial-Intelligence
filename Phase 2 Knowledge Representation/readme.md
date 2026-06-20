# Phase 2: Knowledge Representation 🌾🤖

## 1. Project Summary
As part of my academic coursework in **Artificial Intelligence (SECJ3553)**, our team engineered a formal **Knowledge Representation Framework** to translate messy, highly volatile environmental variables into computer-friendly symbolic logic. The primary challenge addressed in this phase was the complete inability of standard programmatic scripts to dynamically process ambiguous farm conditions (such as conflicting trends between soil dryness and sudden impending storm patterns) and transform them into concrete agricultural instructions. Without a structured semantic layout, an autonomous reasoning system cannot safely evaluate complex, multi-variable field situations, which results in system confusion or faulty, rigid recommendations

To solve the limitation, our pipeline maps real-time data inputs into formal machine logic using a dual-modeling approach:
* **First-Order Predicate Logic (FOPL):** Establishes strict mathematical relationships using quantifiers ($\forall$, $\exists$) and relational predicates. We defined operational predicates including HarvestableAge() (e.g., verifying if an 80-day rice crop is mature enough to survive an emergency rescue harvest), OptimalAge() (the peak maturity window for volumetric yield value), FloodRiskHigh(), and RainfallHeavy().
* **Deterministic Production Rules:** Constructs a modular, human-readable hierarchy of "If-Then" logic conditionals. This reasoning engine continuously evaluates data combinations to fire prescriptive decisions—for example, mapping a rule where if any crop reaches harvestable maturity AND localized flood alerts cross critical limits, the system overrides normal scheduling to trigger immediate emergency harvest alerts ($\forall x [Crop(x) \land HarvestableAge(x) \land FloodRiskHigh() \rightarrow SuggestEmergencyHarvest(x)]$).

The resulting knowledge architecture is modular, completely traceable, and easily expandable. This setup allows the system backend to instantly adjust its expected yield curves and emit precise field mitigation instructions as fresh weather API payloads or IoT soil parameters are ingested.

---

## 2. Personal Reflection

**Key Takeaway** 

* **Symbolic Logic Transformation:** This phase taught me how to bridge the gap between human agricultural judgment and symbolic computer logic. I learned how to represent complex real-world variables, like assessing if an underdeveloped crop is mature enough to withstand an emergency rain harvest, as formal mathematical rules using logical connectors ($\land$, $\lor$, $\rightarrow$).
* **Resolving Operational Conflicts:** I gained a deep understanding of how First-Order Predicate Logic (FOPL) and production rules work together to help an automated engine evaluate shifting farm environments. Applying universal ($\forall$) and existential ($\exists$) quantifiers showed me how a system backend can process multi-variable combinations and trigger clear, real-time diagnostic alerts without program crashing.
* **Designing Explainable and Modular Architectures:** I learned the value of maintaining clean modularity when structuring declarative logic. Ensuring that each predicate and rule acts as an isolated, traceable component showed me how to design an open, explainable AI model that can easily scale to incorporate new sensor properties, crop thresholds, or external climate API criteria.

---

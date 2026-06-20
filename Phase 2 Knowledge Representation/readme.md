# Phase 2: Knowledge Representation 🌾🤖

## 1. Project Summary
As part of my academic coursework in **Artificial Intelligence (SECJ3553)**, our team engineered a formal **Knowledge Representation Framework** to translate messy, highly volatile environmental variables into computer-friendly symbolic logic. The primary challenge addressed in this phase was the complete inability of standard programmatic scripts to dynamically process ambiguous farm conditions (such as conflicting trends between soil dryness and sudden impending storm patterns) and transform them into concrete agricultural instructions. Without a structured semantic layout, an autonomous reasoning system cannot safely evaluate complex, multi-variable field situations, which results in system confusion or faulty, rigid recommendations

To solve the limitation, our pipeline maps real-time data inputs into formal machine logic using a dual-modeling approach:
* **First-Order Predicate Logic (FOPL):** Establishes strict mathematical relationships using quantifiers ($\forall$, $\exists$) and relational predicates. We defined operational predicates including HarvestableAge() (e.g., verifying if an 80-day rice crop is mature enough to survive an emergency rescue harvest), OptimalAge() (the peak maturity window for volumetric yield value), FloodRiskHigh(), and RainfallHeavy().
* **Deterministic Production Rules:** Constructs a modular, human-readable hierarchy of "If-Then" logic conditionals. This reasoning engine continuously evaluates data combinations to fire prescriptive decisions—for example, mapping a rule where if any crop reaches harvestable maturity AND localized flood alerts cross critical limits, the system overrides normal scheduling to trigger immediate emergency harvest alerts ($\forall x [Crop(x) \land HarvestableAge(x) \land FloodRiskHigh() \rightarrow SuggestEmergencyHarvest(x)]$).

The resulting knowledge architecture is modular, completely traceable, and easily expandable. This setup allows the system backend to instantly adjust its expected yield curves and emit precise field mitigation instructions as fresh weather API payloads or IoT soil parameters are ingested.

---

## 2. Personal Reflection

**Name:** Chew Chiu Xian  
**Course:** Artificial Intelligence (SECJ3553 - Section 03)  
**Project Component:** Phase 2 — Knowledge Representation

* Moving into Phase 2 allowed me to bridge the gap between high-level project goals and exact machine reasoning. Before this assignment, I viewed artificial intelligence primarily through raw statistical numbers and black-box calculations. Building our own predicate logic models and production rules taught me how to take abstract human experiences—like a farmer determining if an immature field is worth saving from a heavy storm—and organize them into strict mathematical truths. Mapping variables like crop age thresholds and real-time flood indicators into symbolic equations using logic connectors ($\land$, $\lor$, $\rightarrow$) showed me how a software backend can systematically "think" through real-world contradictions without failing.

* My core focus during this phase was maintaining structural clarity and modularity across our relational rules. I collaborated with my team to define clear logic boundaries, making sure that each predicate was isolated enough to allow new environmental variables or crop types to be introduced without breaking the main system logic. Overcoming the challenge of writing precise conditional statements taught me that a scalable AI system must possess an open, explainable reasoning layer, ensuring that every recommendation pushed to a farmer's dashboard can be tracked back to clear data rules.

---

# Top Mass Diversion Events Dashboard

## Overview

This dashboard provides an interactive view of **major mass diversion events in the U.S. domestic aviation system (July 2021–December 2024)**. It focuses on short time windows where a large number of flights were diverted concurrently from a single airport.

The tool is part of the **[Center for Air Transportation Resilience (CATRes)](https://catres.berkeley.edu/) diversions workstream**, and is designed to support analysis of **system-wide disruption dynamics, airport roles, and network resilience**.

👉 **Live dashboard:**
[https://catres-diversions.github.io/diversion-topcluster-dashboard/](https://catres-diversions.github.io/diversion-topcluster-dashboard/) *(update if needed)*

---

## Purpose

This dashboard zooms in on **specific high-impact events**. It enables users to:

* Examine how diversions concentrate around a **primary planned destination airport (mass diversion center)**
* Trace how flights are redistributed to **diverted-to airports**
* Understand how local diversions are linked to **other planned destination airports across the network**
* Explore **route-level patterns** during mass-diversion windows

---

## How to Use

### 1. Event Selection (Top Right)

* Select a **mass diversion event** from the dropdown list
* Each event corresponds to:

  * a primary planned destination (e.g., DFW)
  * a defined time window

*Note: the list only contains top 5 events for now. We will expand the list to top 20 events.*

---

### 2. View Modes

Two views are available:

* **Diversions Planned for Mass Diversion Center**

  * Shows only flights originally scheduled to the selected airport (e.g., DFW) that were diverted
  * Useful for understanding how diversions affect a specific airport

* **All Diversions in the National Airspace System (NAS)**

  * Shows all diverted flights across the U.S. NAS during the same time window
  * Useful for understanding **system-wide patterns**

---

### 3. Map Visualization

The map shows flight paths and airport roles during the selected event.

**Nodes:**

* 🟡 **Planned destination (mass diversion center)**
* 🔴 **Diverted-to airports** (where flights actually landed)
* ⚪ **Origin airports**

**In system-wide view:**

* 🟢 **Other destination airports affected by diversions in the network**

**Arcs:**

* Lines represent diverted flight paths
* Color indicates airline

---

### 4. Cluster Summary Panel

Provides key metrics for the selected event:

* **Flights planned for the focal airport (mass diversion center) that were diverted**
* **Total diverted flights (system-wide)**
* **Share of system associated with the focal airport**
* **Other planned destination airports affected**
* **Number of origin airports**
* **Number of diverted-to airports**
* **Most common diverted-to airport**

These metrics help distinguish between:

* **localized diversions** (focused on one airport)
* **system-wide events** (affecting many airports)

---

### 5. Airlines Panel

Shows airline activity within the selected event:

* Number of diverted flights by airline
* Relative contribution to the event

**Interpretation:**

* Identifies which airlines are most affected
* Highlights differences in network exposure


---

### 6. Map Layers

Users can toggle visibility of:

* Flight arcs
* Origin airports
* Diverted-to airports
* Planned destination airports

---

## Data Notes

* Data are event-based and extracted from **identified local mass-diversion time windows**
* Each event is defined by:

  * a primary planned destination airport (mass-diversion event center)
  * a start and end time
* Values represent **counts of diverted flights**
* Flight paths are constructed from:

  * origin airport
  * planned destination airport
  * diverted-to airport

---

## Contact

For questions or feedback, please contact CATRes Diversions Project:

* Jasmine Siyu Wu ([jsiyuwu@upenn.edu](mailto:jsiyuwu@upenn.edu))
* Jing Xu ([jing-xu@berkeley.edu](mailto:jing-xu@berkeley.edu))
* Jun Luu ([jjluu@upenn.edu](mailto:jjluu@upenn.edu))

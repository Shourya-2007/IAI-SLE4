# Graph Search Performance Study: BFS vs. DFS (SLE-4)

This repository contains the Architecture Decision Record (ADR), empirical profiling reports, and C4 architecture documentation comparing **Breadth-First Search (BFS)** and **Depth-First Search (DFS)**.

## Project Overview
* **Course:** 02AML204 – Introduction to Artificial Intelligence
* **Student Name:** Shourya Prakash Morbale
* **PRN:** 25UAM051
* **Division:** A
* **Date:** October 2026
* **GitHub Repository:** [IAI-SLE4](https://github.com/Shourya-2007/IAI-SLE4.git)

---

## Repository Structure
* `README.md`: Project documentation and execution overview.
* `CONTRIBUTION.md`: Comprehensive contribution log across the SLE journey.
* `ADR_Defense.md`: Architecture Decision Record (ADR) justifying the selection of DFS.
* `profiling_report/`: Empirical timing results using Python's `timeit` module.
* `architecture/`: Complete 4-level C4 architectural breakdown (Context, Containers, Components, Code Map).

---

## Methodology & Benchmark Configuration
* **Graph Structure:** 100-node sequential adjacency graph starting from node 0.
* **Test Cases:** Evaluated across three distinct goal positions:
  * **Best Case:** Goal 1
  * **Average Case:** Goal 50
  * **Worst Case:** Goal 99
* **Profiling Rigor:** Executed via Python's `timeit` module across three timing runs to record execution times and node expansions accurately.

---

## Summary of Findings (ADR Decision)
* **DFS Selection Status:** Accepted as the preferred traversal algorithm for this benchmark configuration due to measured performance advantages in average and worst-case scenarios.
* **Performance Metrics:**
  * **Best Case (Goal 1):** DFS recorded a lower average execution time of **0.147 ms** compared to BFS at **0.186 ms** (both expanding 2 nodes).
  * **Average Case (Goal 50):** DFS required **1.031 ms** (21 nodes expanded) vs. BFS at **2.451 ms** (51 nodes expanded).
  * **Worst Case (Goal 99):** DFS required **2.129 ms** (43 nodes expanded) vs. BFS at **5.328 ms** (100 nodes expanded).

---

## AI Contribution Note
* **AI Tool Used:** Gemini
* **Assistance Scope:** Assisted in preparing the BFS and DFS profiling code, setting up `timeit` execution-time measurements, adding node-counting logic, and structuring technical reports.
* **Student Contribution:** Executed the program locally, performed three timing runs for each algorithm, collected actual experimental results, verified output metrics, and conducted individual analysis.
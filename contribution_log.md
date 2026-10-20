# Contribution Log – SLE Journey (SLE-1 to SLE-4)

* **Student Name:** Shourya Prakash Morbale
* **PRN:** 25UAM051
* **Course:** 02AML204 – Introduction to Artificial Intelligence
* **Division:** A
* **Project Repository:** [IAI-SLE4](https://github.com/Shourya-2007/IAI-SLE4.git)

---

## Task Breakdown Across SLE Journey

### SLE-1: Foundation & Assistant Setup
* Planned the concept and purpose of the AI Agent for coding and project assistance.
* Set up the local Python development environment and installed required libraries.
* Integrated the Google Gemini API, using a `.env` file to securely manage API keys.
* Developed the core communication script and added robust error handling for environment configurations.
* Tested query execution and created documentation and project interface elements.

### SLE-2: Empirical Profiling & Benchmarking
* Implemented the 100-node sequential adjacency graph benchmark using Python.
* Integrated Python's `timeit` module across three execution runs per test case to measure runtime and node expansion.
* Collected and analyzed actual experimental performance metrics across Best (Goal 1), Average (Goal 50), and Worst (Goal 99) cases.

### SLE-3: Architectural Design (C4 Model)
* Structured the entire system into a complete 4-level C4 architectural model:
  * **Level 1 (System Context):** Mapped system boundary, student actor, and Python runtime dependencies.
  * **Level 2 (Container Architecture):** Separated responsibilities into Graph Setup, Search Services, Experiment Driver, Traversal State, and Measurement & Report.
  * **Level 3 (Component View):** Detailed the Search Services container into BFS (`collections.deque` FIFO queue) and DFS (Python list LIFO stack) components.
  * **Level 4 (Code / Function Map):** Formatted function mappings for `bfs()`, `dfs()`, and `profile_algorithm()`.

### SLE-4: Architecture Decision Record (ADR) & Defense
* Consolidated empirical profiling results into a formal Architecture Decision Record (ADR) justifying the choice of DFS.
* Formulated key performance and architectural talking points in preparation for the oral viva defense.
* Structured final repository code, compiled the contribution history, and generated `README.md`.

---

## Statement of Independence
* **AI Tool Usage:** Utilized Gemini for profiling code templates, timing logic (`timeit`), node-counting structures, and report formatting support.
* **Student Validation:** Personally executed all test scripts locally, completed three timing runs, collected empirical metrics, verified algorithm behaviors, and performed all analytical evaluation.
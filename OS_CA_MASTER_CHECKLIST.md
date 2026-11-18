# Operating Systems Continuous Assessment (CA1–CA7)
## Master Inspection Report & Rubric Mapping Checklist

> **Student Profile:** 2nd-Year Artificial Intelligence & Machine Learning (AI/ML) Undergraduate  
> **Technical Background:** Comfortable with basic Python and Java; beginner in Rust; operating on Windows 11  
> **Assessment Scope:** Complete Continuous Assessment Portfolio (CA1 through CA7) — Total: 70 Marks  
> **Workspace Path:** `C:\Users\Vanshika\Downloads\Academics\OS cloned\Operating-System-Concepts`  
> **Inspection Status:** Complete Codebase and Syllabus Audit; No original files modified or deleted  
> **Date of Inspection:** November 2026  

---

## 1. Executive Summary & Assessment Overview

The Operating Systems Continuous Assessment framework is a progressive, 7-tier systems-engineering portfolio replacing traditional exams with evidence-based problem solving, measurement, debugging, research, Linux systems administration, and bare-metal kernel development.

### Complete 70-Mark Continuous Assessment Architecture
*(Source: `Activities-and-Assignments/CA7_OS_Engineering_Viva_and_Demonstration.md` §40–42)*

| CA Identifier | Title | Marks | Central Question | Core Capability | Primary Language / Platform |
|---|---|:---:|---|---|---|
| **CA-1** | OS Systems Thinking Challenge | 10 | *"What is the OS problem?"* | Understand, Model, Reason, Decide, Justify | Written Analysis / Python helper |
| **CA-2** | OS Performance Investigation | 10 | *"What does experimental evidence show?"* | Measure, Benchmark, Compare, Interpret | Python 3.x (Optional: Rust) |
| **CA-3** | OS Design & Debugging Challenge | 10 | *"Why did it fail & how can it be fixed?"* | Diagnose, Model, Fix, Regress-Test | Python 3.x (Optional: Rust) |
| **CA-4** | OS Research Mini-Project | 10 | *"What is not yet completely answered?"* | Literature Review, Hypothesize, Experiment | Python 3.x (Optional: Rust) |
| **CA-5** | Linux Systems Engineering Challenge | 10 | *"How does the real OS behave?"* | Instrument, Control, Intervene on Real Linux | Bash + Python 3.x on Linux / WSL |
| **CA-6** | Rust Micro-OS Engineering Project | 15 | *"Can I implement OS mechanisms myself?"* | Systems Construction, Kernel Architecture | Rust (`no_std`) + QEMU + Cargo |
| **CA-7** | OS Engineering Viva & Demonstration | 5 | *"Can I explain and defend my decisions?"* | Live Demonstration, Adaptive Defence | Oral Viva / Live Demo (All CAs) |
| **TOTAL** | **Continuous Assessment Portfolio** | **70** | | **Full Engineering Lifecycle** | |

### Pedagogical Progression
```text
CA-1: Systems Thinking (Think) ──► CA-2: Performance (Measure) ──► CA-3: Debugging (Engineer)
                                                                            │
CA-6: Rust Micro-OS (Build) ◄── CA-5: Linux Systems (Observe) ◄── CA-4: Research (Investigate)
             │
             ▼
CA-7: Viva & Demonstration (Defend 70 Marks)
```

---

## 2. Deliverable 1: CA-by-CA Requirement Tables

---

### CA-1: OS Systems Thinking Challenge (10 Marks)
*Primary Reference: `Activities-and-Assignments/CA1_Systems_Thinking_Challenge.md`*

| Aspect | Specific Requirement & Citation |
|---|---|
| **Problem / Challenge** | Scenario-based, analytical, decision-oriented engineering evaluation (§1). Students evaluate a realistic computing scenario exhibiting bottlenecks, race conditions, or resource contention, identify the underlying OS mechanism, and defend an engineering decision. |
| **Mandatory Implementation Requirements** | Follow the mandatory 5-stage student thinking framework (§5–9):<br>1. *Identify OS Concept*: State subsystem and explain why (§5).<br>2. *Model the Problem*: Diagram, queue model, state machine, or mathematical formulation (§6).<br>3. *Analyze Alternatives*: Critically evaluate at least two plausible OS mechanisms (§7).<br>4. *Select Mechanism*: Explicit engineering decision based on constraints (§8).<br>5. *Justify Decision*: Defend with calculations, traces, or evidence (§9). |
| **Programming Language & Tools** | Analytical writing; Python 3.x standard library for optional calculations, simulation traces, or verification scripts (§8, §10). LaTeX or Markdown formatting. |
| **Expected Submission Deliverables** | An Engineering Decision Document (§10, §25) following the 11-section template:<br>A. Scenario Understanding, B. OS Concept Identification, C. System Model, D. Constraints & Assumptions, E. Alternative Solutions, F. Comparative Analysis, G. Selected Solution, H. Engineering Justification, I. Trade-offs & Limitations, J. AI Corroboration Record, K. Final Engineering Decision. |
| **Required Experiments & Test Cases** | Numerical or trace-based comparison under changing workload constraints (e.g., interactive vs batch, varying arrival/burst profiles, multi-core scaling) (§7, §9). |
| **Evidence & Screenshots** | Execution traces, ASCII/Mermaid architectural models, Gantt charts, calculation tables, or small script output (§6, §9, §15). |
| **Marking Criteria & Marks** | **Total: 10 Marks** (§4, §17):<br>1. *OS Concept Identification*: 2 Marks<br>2. *Problem Modelling*: 2 Marks<br>3. *Alternative Analysis*: 2 Marks<br>4. *Mechanism Selection*: 2 Marks<br>5. *Justification & Communication*: 2 Marks |

---

### CA-2: OS Performance Investigation (10 Marks)
*Primary Reference: `Activities-and-Assignments/CA2_Performance_Investigation.md`*

| Aspect | Specific Requirement & Citation |
|---|---|
| **Problem / Challenge** | Evidence-based performance investigation (§1). Formulate a measurable performance question, predict behaviour with a testable hypothesis, generate controlled workloads, and collect quantitative benchmark metrics (§5–6). |
| **Mandatory Implementation Requirements** | Must follow 9-step workflow (§5–13):<br>1. Define research question.<br>2. Formulate testable hypothesis.<br>3. Classify Independent, Dependent, and Controlled variables (§7).<br>4. Implement controlled simulator/benchmark.<br>5. Execute experiments with multiple input sizes, multiple parameter values, and at least 3 repetitions per measurement (§9).<br>6. Retain raw observations in structured tables (§10).<br>7. Generate visualizations with interpretation (§11).<br>8. Account for experimental noise (§17).<br>9. Provide evidence-based recommendation (§13). |
| **Programming Language & Tools** | **Python 3.x** (recommended default for algorithmic OS simulations, data processing, and plotting via matplotlib/seaborn or standard library) (§8, §24). Rust optional for low-level thread comparison. |
| **Expected Submission Deliverables** | Structured Technical Report (18 sections, §19): Title, Question, Objective, Concept, Hypothesis, Environment, Variables, Methodology, Implementation, Workloads, Raw Results, Analysis, Visualization, Discussion, Decision, Limitations, AI Disclosure, Conclusion. |
| **Required Experiments & Test Cases** | At least 3 workload types (e.g., CPU-bound, I/O-oriented, Mixed) (§14 Exp 1); multiple parameter levels (e.g., Round Robin quantum at 1, 5, 10, 20, 50, 100 ms); minimum 3–5 repeated runs per data point (§9). |
| **Evidence & Screenshots** | Structured numerical tables (raw + summarized), performance curves/bar charts/box plots, environment documentation table (CPU, OS, RAM, Python version) (§9–11). |
| **Marking Criteria & Marks** | **Total: 10 Marks** (§4, §21):<br>1. *Experimental Design & Methodology*: 2 Marks<br>2. *Implementation & Correctness*: 2 Marks<br>3. *Data Collection & Measurement*: 2 Marks<br>4. *Analysis & Visualization*: 2 Marks<br>5. *Engineering Interpretation & Conclusion*: 2 Marks |

---

### CA-3: OS Design & Debugging Challenge (10 Marks)
*Primary Reference: `Activities-and-Assignments/CA3_Design_and_Debugging_Challenge.md`*

| Aspect | Specific Requirement & Citation |
|---|---|
| **Problem / Challenge** | Engineering intervention on defective/inefficient/unsafe OS-related software (§1). Diagnose an underlying OS fault (race condition, deadlock, starvation, bad state transition, fragmentation, etc.), identify the root cause, design and implement an OS-principled fix, and prove the fix works (§5–11). |
| **Mandatory Implementation Requirements** | Follow the 7-stage debugging framework (§5–11):<br>1. *Observe Failure*: Document reproducing symptom.<br>2. *Identify OS Concept*: Explain violated OS principle (§6).<br>3. *Model Failure*: State diagram, resource allocation graph, or execution trace (§7).<br>4. *Determine Root Cause*: Distinguish symptom from root cause (§8).<br>5. *Analyze Alternatives*: Compare at least two corrective designs (§9).<br>6. *Implement & Validate*: Write clean, tested fix (§10).<br>7. *Regression Testing*: Prove failure is eliminated without breaking prior features (§11, §20). |
| **Programming Language & Tools** | **Python 3.x** (default for simulation/algorithm bugs); Bash + Python for Linux environment bugs; Rust for advanced concurrency/memory safety bugs (§10). |
| **Expected Submission Deliverables** | Debugging and Design Response Report (12 sections, §18): Problem Statement, OS Concept, Failure Reproduction, System Model, Root Cause, Alternative Solutions, Selected Design, Implementation, Validation, Trade-off Analysis, AI Disclosure, Final Defence. Accompanying source code before and after fix. |
| **Required Experiments & Test Cases** | 5 distinct test classes (§19):<br>1. Normal operating case<br>2. Boundary case (min/max parameters)<br>3. Stress case (high concurrency/load)<br>4. Adversarial case (trigger edge conditions)<br>5. Recovery case / Regression suite (Before vs After comparison) (§20). |
| **Evidence & Screenshots** | Reproducible terminal failure logs (Before), debugger/trace logs, corrected execution logs (After), comparative execution timings or resource usage profiles (§11, §18). |
| **Marking Criteria & Marks** | **Total: 10 Marks** (§4, §22):<br>1. *Problem Diagnosis & Root-Cause Identification*: 2 Marks<br>2. *System/Algorithm Modelling & Reasoning*: 2 Marks<br>3. *Solution Design & Alternative Analysis*: 2 Marks<br>4. *Implementation & Validation*: 2 Marks<br>5. *Technical Defence, Trade-offs & Communication*: 2 Marks |

---

### CA-4: OS Research Mini-Project (10 Marks)
*Primary Reference: `Activities-and-Assignments/CA4_Research_Mini_Project.md`*

| Aspect | Specific Requirement & Citation |
|---|---|
| **Problem / Challenge** | Small-scale, evidence-based research on an unanswered or comparative OS question (§1). Formulate a focused research problem, review academic literature, identify a research gap, implement a simulator/benchmark, and defend findings (§2, §5). |
| **Mandatory Implementation Requirements** | 1. Research Ladder Level: Must achieve at least Level 2 (Compare) or Level 3 (Extend) (§4).<br>2. Literature Review: Minimum 3–5 credible references with at least 2 research papers (§13).<br>3. Mandatory Literature Matrix (§34).<br>4. Pre-implementation Faculty Approval Checkpoint (§22).<br>5. Explicit variable isolation: Independent, Dependent, Controlled, Environmental (§10).<br>6. Threats to Validity: Identify at least two internal/external limitations (§18). |
| **Programming Language & Tools** | **Python 3.x** (default for algorithm simulation, synthetic workload generation, and statistical visualization) (§6); Python + Linux for systems metrics; Rust encouraged for low-level systems research. |
| **Expected Submission Deliverables** | Complete Research Package (§33):<br>1. Research proposal (§14)<br>2. Literature matrix table (§34)<br>3. Prototype source code<br>4. Experimental configuration & raw datasets<br>5. Processed data & analytical plots<br>6. Final Research Report (18 sections, §15)<br>7. AI Disclosure (§12)<br>8. Short demonstration slides/viva readiness. |
| **Required Experiments & Test Cases** | Baseline workload vs parameter variation across repeated runs (5–10 runs per condition) (§10); statistical variance/confidence checks (box plots or mean ± std dev); synthetic workload sweeps. |
| **Evidence & Screenshots** | Literature matrix, performance curves, raw CSV logs, statistical graphs, reproducibility documentation (§11, §16, §17). Screenshots alone are strictly forbidden as primary evidence (§16). |
| **Marking Criteria & Marks** | **Total: 10 Marks** (§19):<br>1. *Research problem, question & gap*: 2 Marks<br>2. *Literature review & research justification*: 1 Mark<br>3. *Experimental methodology & design*: 2 Marks<br>4. *Prototype/implementation & correctness*: 1 Mark<br>5. *Data collection, analysis & visualization*: 2 Marks<br>6. *Research interpretation, limitations & conclusion*: 1 Mark<br>7. *Technical communication & AI-use disclosure*: 1 Mark |

---

### CA-5: Linux Systems Engineering Challenge (10 Marks)
*Primary Reference: `Activities-and-Assignments/CA5_Linux_Systems_Engineering_Challenge.md`*

| Aspect | Specific Requirement & Citation |
|---|---|
| **Problem / Challenge** | Real-system observation, control, instrumentation, and engineering on Linux (§1). Observe internal kernel data structures via `/proc`, manipulate processes, signals, scheduling priorities (`nice`), CPU affinity (`taskset`), or memory behavior, and engineer an intervention (§3, §4). |
| **Mandatory Implementation Requirements** | Follow the 9-stage engineering framework (§4): Observe ➔ Formulate ➔ Instrument ➔ Experiment ➔ Control ➔ Analyze ➔ Engineer ➔ Validate ➔ Defend.<br>Must adhere to the Minimum Evidence Rule (§22): **Baseline ➔ Intervention ➔ Measurement ➔ Comparison ➔ Conclusion**.<br>Must strictly follow Laboratory Safety Rules (§24): No host fork bombs, no destructive disk filling, no killing unauthorized processes. |
| **Programming Language & Tools** | **Linux Environment** (WSL 2 / Ubuntu VM / Native Linux). **Bash** for command-line orchestration; **Python 3.x** for automation, `/proc` parsing, and data logging (§5, §6). Linux toolchain: `ps`, `top`/`htop`, `/proc/<pid>/`, `pidstat`, `vmstat`, `iostat`, `free`, `lscpu`, `taskset`, `nice`/`renice`, `strace`. |
| **Expected Submission Deliverables** | Linux Engineering Submission Package (§37): Problem Statement, OS Mechanism Explanation, Linux Environment Specification, Bash/Python Source Code, Executed Commands Log, Raw Measurements, `/proc` Inspection Traces, Comparative Visualizations, Engineering Intervention Log, Validation Evidence, Limitations, AI Disclosure. |
| **Required Experiments & Test Cases** | Controlled execution comparing Baseline vs Intervened state (e.g., Unpinned vs Pin-to-Core execution; Default nice vs Reniced priority; Unbuffered vs Buffered pipe I/O) across varying workloads (§8–17). |
| **Evidence & Screenshots** | Verifiable terminal logs showing command execution, `/proc/<pid>/stat` or `/proc/<pid>/status` snapshots, `taskset` / `renice` output, before-and-after throughput/latency metrics (§9, §22). |
| **Marking Criteria & Marks** | **Total: 10 Marks** (§7, §27):<br>1. *Problem & OS Understanding*: 2 Marks<br>2. *Linux Instrumentation & Tool Usage*: 2 Marks<br>3. *Engineering Intervention*: 2 Marks<br>4. *Evidence & Analysis*: 2 Marks<br>5. *Validation & Defence*: 2 Marks |

---

### CA-6: Rust Micro-OS Engineering Project (15 Marks)
*Primary Reference: `Activities-and-Assignments/CA6_Rust_Micro_OS_Engineering_Project.md`*

| Aspect | Specific Requirement & Citation |
|---|---|
| **Problem / Challenge** | Flagship systems construction project (§1). Design and build a minimal, educational Micro-OS kernel in **Rust** running in an emulator (QEMU), implementing core kernel mechanisms (boot, console, tasks, scheduler, timer, synchronization, memory) plus one chosen specialization track (§3, §4, §8). |
| **Mandatory Implementation Requirements** | 1. **Core Subsystems (Mandatory for all)** (§4, §10):<br>&nbsp;&nbsp;• Layer 1: Rust bare-metal kernel boot entry (§9)<br>&nbsp;&nbsp;• Layer 2: Kernel console / UART serial output & diagnostics<br>&nbsp;&nbsp;• Layer 3: Task representation (`READY`, `RUNNING`, `BLOCKED`, `TERMINATED`)<br>&nbsp;&nbsp;• Layer 4: Ready Queue data structure<br>&nbsp;&nbsp;• Layer 5: Round Robin CPU scheduler<br>&nbsp;&nbsp;• Layer 6: Timer-driven scheduling trigger<br>&nbsp;&nbsp;• Layer 7: Kernel synchronization primitive (spinlock or mutex)<br>&nbsp;&nbsp;• Layer 8: Memory allocation mechanism (bump, free-list, or fixed-block allocator)<br>&nbsp;&nbsp;• Layer 10: Integrated kernel execution demo.<br>2. **Specialization Track**: Choose exactly one track from §11 (e.g., Track A: Priority/MLFQ Scheduler, Track B: Allocator/Paging, Track C: Lock Contention, Track D: Syscalls).<br>3. **`unsafe` Rust Policy**: Every `unsafe` block must state reason, assumptions, and invariants (§26). |
| **Programming Language & Tools** | **Rust** (`no_std`, stable or nightly depending on bootloader target), `cargo`, `rustup`, target components (e.g. `x86_64-unknown-none`), **QEMU** (`qemu-system-x86_64`), Python for serial log parsing and trace analysis, Git (§6, §7, §19). |
| **Expected Submission Deliverables** | Final Submission Package (§42):<br>1. Rust Micro-OS source repository (Cargo workspace, `src/`, `Cargo.toml`)<br>2. Architecture document with Data/Control Flow Diagram (§24)<br>3. Design document & `unsafe` audit log (§26)<br>4. Test plan & validation results (§15, §16)<br>5. Python analysis scripts & performance traces (§19)<br>6. Debugging log (§21)<br>7. Final technical report (20 sections, §23)<br>8. Live QEMU demonstration<br>9. Individual contribution statement (§31)<br>10. AI usage disclosure (§25). |
| **Required Experiments & Test Cases** | 6 mandatory test cases (§16):<br>• TC1: Minimum Configuration (2 tasks)<br>• TC2: Multiple Tasks (3–5 concurrent tasks)<br>• TC3: Boundary Case (smallest meaningful quantum / memory chunk)<br>• TC4: Stress Case (high task count / rapid allocations)<br>• TC5: Failure Case (controlled invalid operation / memory exhaustion rejection)<br>• TC6: Repeatability Test (identical repeated trace run). |
| **Evidence & Screenshots** | QEMU boot window screenshot, serial port / console logs showing task preemption and scheduling transitions, trace plots (Python-generated task Gantt charts from serial output), memory allocation statistics (§17, §18). |
| **Marking Criteria & Marks** | **Total: 15 Marks** (§28, §29):<br>1. *Architecture and OS Mechanism Design*: 2 Marks<br>2. *Rust Implementation Quality*: 4 Marks<br>3. *Core OS Functionality*: 3 Marks<br>4. *Testing, Debugging and Validation*: 2 Marks<br>5. *Performance/Evidence-Based Evaluation*: 2 Marks<br>6. *Innovation / Specialization*: 1 Mark<br>7. *Documentation and Technical Demonstration*: 1 Mark |

---

### CA-7: OS Engineering Viva & Demonstration (5 Marks)
*Primary Reference: `Activities-and-Assignments/CA7_OS_Engineering_Viva_and_Demonstration.md`*

| Aspect | Specific Requirement & Citation |
|---|---|
| **Problem / Challenge** | Comprehensive individual oral defence and live demonstration (§1). Defend engineering choices, interpret evidence, diagnose live modified scenarios, and justify trade-offs across the entire CA1–CA6 portfolio (§3, §5). |
| **Mandatory Implementation Requirements** | 1. Live demonstration of at least one functional artifact (preferably CA-6 Micro-OS or CA-5 Linux tool) (§8).<br>2. Individual questioning following the 7-level adaptive viva model: Level 1 Demonstrate ➔ Level 2 Explain ➔ Level 3 Modify ➔ Level 4 Break ➔ Level 5 Diagnose ➔ Level 6 Justify ➔ Level 7 Extend (§6).<br>3. Respond to "Break My System" controlled fault injection (§26).<br>4. Defend AI disclosure and verify independent understanding (§27). |
| **Programming Language & Tools** | Running live software on student machine (QEMU, Python, Terminal), architecture diagrams, code walkthrough (§5, §45). |
| **Expected Submission Deliverables** | Prepared portfolio brought to viva (§45):<br>1. Executable Micro-OS and Linux scripts ready to run<br>2. Architecture and design diagrams<br>3. Experimental results and data charts<br>4. Debugging log highlighting critical resolutions<br>5. Faculty Viva Record Sheet completion (§43). |
| **Required Experiments & Test Cases** | Live execution under altered parameters (e.g., modifying task quantum, injecting shared resource conflict, or explaining memory exhaustion behavior on the fly) (§6, §25, §26). |
| **Evidence & Screenshots** | Real-time live execution during the 8–12 minute viva session; faculty evaluation recorded on Faculty Viva Record Sheet (§5, §43). |
| **Marking Criteria & Marks** | **Total: 5 Marks** (§7, §31):<br>1. *Technical Demonstration*: 1 Mark<br>2. *Conceptual Understanding*: 1 Mark<br>3. *Engineering Reasoning & Trade-offs*: 1 Mark<br>4. *Debugging / Scenario-Based Questioning*: 1 Mark<br>5. *Communication, Individual Contribution & Defence*: 1 Mark |

---

## 3. Deliverable 2: Granular Rubric Checklist

This checklist converts every single assessment criterion into granular, verified tasks.

### CA-1 Rubric Checklist (10 Marks Total)
- [ ] **Criterion 1: OS Concept Identification (2 Marks)** *(Ref: CA1 §17)*
  - [ ] Accurately name the primary OS subsystem and concept (e.g., CPU Scheduling, Virtual Memory Thrashing, Deadlock). [1 Mark]
  - [ ] Provide contextual reasoning explaining why the scenario represents this OS mechanism rather than a generic software flaw. [1 Mark]
- [ ] **Criterion 2: Problem Modelling (2 Marks)** *(Ref: CA1 §17)*
  - [ ] Construct a technical model appropriate to the domain (e.g., Gantt chart, process state diagram, Resource Allocation Graph, page reference string). [1 Mark]
  - [ ] Accompany the model with clear annotations, parameter definitions, and assumptions. [1 Mark]
- [ ] **Criterion 3: Alternative Analysis (2 Marks)** *(Ref: CA1 §17)*
  - [ ] Present at least two distinct, plausible OS mechanisms that could address the situation. [1 Mark]
  - [ ] Critically compare the alternatives using quantitative criteria (e.g., waiting time, context switch overhead, fragmentation). [1 Mark]
- [ ] **Criterion 4: Mechanism Selection (2 Marks)** *(Ref: CA1 §17)*
  - [ ] Explicitly state the selected OS mechanism and configuration parameters. [1 Mark]
  - [ ] Align the selection directly with the stated system constraints and workload characteristics. [1 Mark]
- [ ] **Criterion 5: Justification & Communication (2 Marks)** *(Ref: CA1 §17)*
  - [ ] Defend the decision using concrete calculations, traces, or technical citations. [1 Mark]
  - [ ] Detail trade-offs, limitations, and conditions under which the decision would change, with verified AI disclosure. [1 Mark]

### CA-2 Rubric Checklist (10 Marks Total)
- [ ] **Criterion 1: Experimental Design & Methodology (2 Marks)** *(Ref: CA2 §21)*
  - [ ] State a clear, testable research question and predictive hypothesis. [1 Mark]
  - [ ] Explicitly classify and control Independent, Dependent, and Controlled variables. [1 Mark]
- [ ] **Criterion 2: Implementation & Correctness (2 Marks)** *(Ref: CA2 §21)*
  - [ ] Implement the core OS algorithm/simulator correctly in Python 3.x. [1 Mark]
  - [ ] Validate algorithm correctness against known analytical baselines across multiple workload types. [1 Mark]
- [ ] **Criterion 3: Data Collection & Measurement (2 Marks)** *(Ref: CA2 §21)*
  - [ ] Execute controlled experiments across multiple input sizes/parameters with at least 3 repetitions per measurement. [1 Mark]
  - [ ] Maintain complete raw and aggregated data tables documenting hardware/software environment. [1 Mark]
- [ ] **Criterion 4: Analysis & Visualization (2 Marks)** *(Ref: CA2 §21)*
  - [ ] Generate clear, properly labelled visual charts (line, bar, box plots) displaying performance trends. [1 Mark]
  - [ ] Provide written analytical commentary explaining the trends and isolating experimental noise. [1 Mark]
- [ ] **Criterion 5: Engineering Interpretation & Conclusion (2 Marks)** *(Ref: CA2 §21)*
  - [ ] Formulate an evidence-based conclusion confirming or refuting the hypothesis. [1 Mark]
  - [ ] Discuss workload-dependent trade-offs and define operational boundaries for the recommendation. [1 Mark]

### CA-3 Rubric Checklist (10 Marks Total)
- [ ] **Criterion 1: Problem Diagnosis & Root-Cause Identification (2 Marks)** *(Ref: CA3 §22)*
  - [ ] Faithfully reproduce the failure and document observable symptoms. [1 Mark]
  - [ ] Isolate the exact root cause, distinguishing symptoms from the violated OS principle. [1 Mark]
- [ ] **Criterion 2: Modelling & Reasoning (2 Marks)** *(Ref: CA3 §22)*
  - [ ] Create a technical trace or model depicting the defective state (e.g., concurrency interleaving, circular wait graph). [1 Mark]
  - [ ] Mathematically or logically explain why the defect inevitably triggers under concurrency or load. [1 Mark]
- [ ] **Criterion 3: Solution Design & Alternative Analysis (2 Marks)** *(Ref: CA3 §22)*
  - [ ] Propose and evaluate at least two alternative engineering designs to fix the flaw. [1 Mark]
  - [ ] Justify the chosen design based on correctness, overhead, complexity, and scalability. [1 Mark]
- [ ] **Criterion 4: Implementation & Validation (2 Marks)** *(Ref: CA3 §22)*
  - [ ] Implement the fix cleanly in Python 3.x / Rust without side effects. [1 Mark]
  - [ ] Execute a 5-part test suite (normal, boundary, stress, adversarial, recovery) demonstrating fix effectiveness. [1 Mark]
- [ ] **Criterion 5: Technical Defence & Regression Testing (2 Marks)** *(Ref: CA3 §22)*
  - [ ] Execute regression testing comparing Before vs After states across correctness and performance. [1 Mark]
  - [ ] Defend introduced trade-offs (e.g., lock contention overhead) with verified AI disclosure. [1 Mark]

### CA-4 Rubric Checklist (10 Marks Total)
- [ ] **Criterion 1: Research Problem, Question & Gap (2 Marks)** *(Ref: CA4 §19)*
  - [ ] Formulate a specific, measurable OS research problem narrower than a general textbook topic. [1 Mark]
  - [ ] Explicitly identify a justified research gap in contemporary systems literature. [1 Mark]
- [ ] **Criterion 2: Literature Review & Justification (1 Mark)** *(Ref: CA4 §19)*
  - [ ] Synthesize 3–5 credible sources, including at least 2 research papers, inside a structured Literature Matrix. [1 Mark]
- [ ] **Criterion 3: Experimental Methodology & Design (2 Marks)** *(Ref: CA4 §19)*
  - [ ] Design a reproducible experimental harness with isolated variables and defined metrics. [1 Mark]
  - [ ] Secure faculty approval through the Stage 4 Approval Checkpoint. [1 Mark]
- [ ] **Criterion 4: Prototype Implementation & Correctness (1 Mark)** *(Ref: CA4 §19)*
  - [ ] Build a functioning prototype/simulator in Python 3.x generating verifiable output. [1 Mark]
- [ ] **Criterion 5: Data Collection, Analysis & Visualization (2 Marks)** *(Ref: CA4 §19)*
  - [ ] Systematically collect experimental data across repeated runs and workloads. [1 Mark]
  - [ ] Produce publication-quality plots illustrating relationships between variables. [1 Mark]
- [ ] **Criterion 6: Research Interpretation, Limitations & Conclusion (1 Mark)** *(Ref: CA4 §19)*
  - [ ] Answer the research question with evidence and explicitly analyze at least two threats to validity. [1 Mark]
- [ ] **Criterion 7: Technical Communication & AI Disclosure (1 Mark)** *(Ref: CA4 §19)*
  - [ ] Author a formal 18-section research report with full citations and an AI verification statement. [1 Mark]

### CA-5 Rubric Checklist (10 Marks Total)
- [ ] **Criterion 1: Problem Understanding & OS Mechanism (2 Marks)** *(Ref: CA5 §27)*
  - [ ] State the specific real-world Linux OS mechanism being investigated. [1 Mark]
  - [ ] Differentiate real kernel behavior from simplified textbook models. [1 Mark]
- [ ] **Criterion 2: Linux Instrumentation & Tool Usage (2 Marks)** *(Ref: CA5 §27)*
  - [ ] Select and execute appropriate Linux system inspection utilities (`/proc`, `ps`, `top`, `pidstat`, `taskset`). [1 Mark]
  - [ ] Script and automate telemetry extraction cleanly using Bash and Python. [1 Mark]
- [ ] **Criterion 3: Engineering Intervention (2 Marks)** *(Ref: CA5 §27)*
  - [ ] Execute a concrete system-level intervention (e.g., CPU affinity binding, priority renicing, pipe buffer tuning). [1 Mark]
  - [ ] Follow laboratory safety guidelines ensuring no host system degradation. [1 Mark]
- [ ] **Criterion 4: Evidence & Analysis (2 Marks)** *(Ref: CA5 §27)*
  - [ ] Present quantitative system evidence conforming to the rule: Baseline ➔ Intervention ➔ Measurement ➔ Comparison. [1 Mark]
  - [ ] Explain observed system responses using kernel-level principles. [1 Mark]
- [ ] **Criterion 5: Validation, Defence & Reproducibility (2 Marks)** *(Ref: CA5 §27)*
  - [ ] Document complete distribution and kernel specifications enabling full reproducibility. [1 Mark]
  - [ ] Defend findings and validate that intervention produced intended effects without regressions. [1 Mark]

### CA-6 Rubric Checklist (15 Marks Total)
- [ ] **Criterion 1: Architecture & OS Mechanism Design (2 Marks)** *(Ref: CA6 §28)*
  - [ ] Produce a modular kernel architectural design diagram detailing data and control flow across boot, scheduler, and memory. [1 Mark]
  - [ ] Justify kernel component separation and hardware abstraction boundaries. [1 Mark]
- [ ] **Criterion 2: Rust Implementation Quality (4 Marks)** *(Ref: CA6 §28)*
  - [ ] Write correct, idiomatic `no_std` Rust utilizing safe abstractions. [2 Marks]
  - [ ] Document all `unsafe` blocks with clear invariants, safety boundaries, and necessity rationales. [2 Marks]
- [ ] **Criterion 3: Core OS Functionality (3 Marks)** *(Ref: CA6 §28)*
  - [ ] Demonstrate bare-metal kernel boot and formatted console/serial logging output. [1 Mark]
  - [ ] Implement task management structs, state transitions, and a working ready queue. [1 Mark]
  - [ ] Implement Round Robin CPU scheduling and a basic memory allocator. [1 Mark]
- [ ] **Criterion 4: Testing, Debugging & Validation (2 Marks)** *(Ref: CA6 §28)*
  - [ ] Execute test cases TC1 through TC6 covering multi-task, boundary, stress, and failure cases. [1 Mark]
  - [ ] Maintain a detailed debugging log recording root causes and resolutions for low-level faults. [1 Mark]
- [ ] **Criterion 5: Performance / Evidence-Based Evaluation (2 Marks)** *(Ref: CA6 §28)*
  - [ ] Capture kernel serial traces and parse them with Python to generate scheduling Gantt charts. [1 Mark]
  - [ ] Quantify task-switch counts, scheduling latency, and memory allocation utilization. [1 Mark]
- [ ] **Criterion 6: Innovation / Specialization Track (1 Mark)** *(Ref: CA6 §28)*
  - [ ] Implement and evaluate one chosen specialization track (e.g., Priority Scheduler or Dynamic Quantum). [1 Mark]
- [ ] **Criterion 7: Documentation & Live Demonstration (1 Mark)** *(Ref: CA6 §28)*
  - [ ] Complete the 20-section technical report and demonstrate the live Micro-OS booting and running in QEMU. [1 Mark]

### CA-7 Rubric Checklist (5 Marks Total)
- [ ] **Criterion 1: Technical Demonstration (1 Mark)** *(Ref: CA7 §31)*
  - [ ] Successfully boot and execute the live software artifact (CA6 Micro-OS in QEMU or CA5 Linux tool) within 2 minutes. [1 Mark]
- [ ] **Criterion 2: Conceptual Understanding (1 Mark)** *(Ref: CA7 §31)*
  - [ ] Articulate underlying OS theory across CO1–CO6 without relying on rote memorization. [1 Mark]
- [ ] **Criterion 3: Engineering Reasoning & Trade-offs (1 Mark)** *(Ref: CA7 §31)*
  - [ ] Justify implementation choices (e.g., Why Round Robin? Why bump allocation?) with reasoned trade-offs. [1 Mark]
- [ ] **Criterion 4: Debugging / Scenario-Based Reasoning (1 Mark)** *(Ref: CA7 §31)*
  - [ ] Successfully analyze and predict outcomes of hypothetical fault injections or parameter changes. [1 Mark]
- [ ] **Criterion 5: Communication, Contribution & Defence (1 Mark)** *(Ref: CA7 §31)*
  - [ ] Defend individual contributions with clarity, confidence, and verified disclosure of AI assistance. [1 Mark]

---

## 4. Deliverable 3: Existing Codebase Inventory & Reuse Analysis

An exhaustive audit of the cloned repository reveals the following assets:

### 1. Reusable Implementations (Fully Implemented Code)
These files contain functional, tested Python or C implementations that can be adapted for experiments:

| Directory | File | Purpose | Reusability in CAs |
|---|---|---|---|
| `Chapter 3.1 - Processes\3.20` | `pid_manager.py` / `.c` | Bitmap-based PID allocation & release | **CA-3**: Can inject race/boundary faults; **CA-6**: Task ID manager. |
| `Chapter 3.1 - Processes\3.19` | `time_pipe.py`, `time_shared_memory.py` | Command execution timing over IPC | **CA-2 / CA-5**: Timing harness for process benchmarking. |
| `Chapter 3.1 - Processes\3.21` | `collatz.py` / `.c` | Process creation via `fork()` | **CA-2 / CA-3**: Process creation baseline; can create zombies. |
| `Chapter 3.1 - Processes\3.26` | `reverse_case.py` / `.c` | Ordinary pipe message exchange | **CA-5**: Pipe IPC baseline. |
| `Chapter 3.2 - UNIX Shell project` | `shell.py` / `shell.c` | Command execution, history, pipes, redirection | **CA-1 / CA-5**: Process control, redirection, and shell mechanics. |
| `Chapter 3.4 - Linux Kernel Module for Listing Tasks` | `process_linear_iteration.py`, `process_dfs.py` | Linux `/proc` traversal & task tree DFS | **CA-5**: Directly reusable starter for `/proc` explorer. |
| `Chapter 3.3 - Linux Kernel Module for Task Information` | `pid.py` | Reading `/proc/<pid>/stat` for state/command | **CA-5**: Direct building block for process inspection. |
| `Chapter 4.1 - Threads & Concurrency` | `4.22\main.py`, `4.24\main.py` | Multithreaded statistical & Monte Carlo computations | **CA-2**: Multithreading benchmarks; **CA-3**: Race condition injection. |
| `Chapter 4.2 - Sudoku Solution Validator` | `main.py` / `main.c` | 11 worker threads validating grid | **CA-2**: Thread concurrency scaling. |
| `Chapter 4.3 - Multithreaded sorting` | `main.py` / `main.c` | Multithreaded merge sort | **CA-2**: Parallel vs serial execution comparison. |
| `Chapter 6 - Synchronization Tools` | `6.33\main.py` / `main.c` | Finite resource manager with mutex locks | **CA-2 / CA-3**: Benchmarking contention or injecting race conditions. |

### 2. Reference-Only Files (Stubs and Tutorials)
- **Chapters 7 through 21 Python files:**  
  All `.py` files in `Chapter-07` through `Chapter-21` (e.g. `7.01_bounded_buffer.py`, `8.01_bankers_algorithm.py`, `9.01_fixed_partitioning.py`, `10.01_fifo_page_replacement.py`, `11.01_disk_scheduling.py`, `20.01_proc_process_monitor.py`) are **starter stubs**. They only print a welcome banner and text stating: *"This starter implementation is intentionally lightweight. Extend the simulation, collect measurements, and discuss the OS concept."* They contain **no algorithmic implementation**.
- **`Chapter 1 - Introduction`**: Contains reference markdown tutorials for basic Unix commands and shell scripting, useful as study references for CA-5.

### 3. Requirements Needing Brand New Implementation
- **CPU Scheduling Algorithms:** Chapter 5 has no directory in the repository. FCFS, SJF, Priority, and Round Robin simulators required for CA-2 (or CA-4) must be built from scratch.
- **Page Replacement & Memory Allocators:** Complete FIFO, LRU, Optimal algorithms, or dynamic partition simulators must be written from scratch if selected.
- **Micro-OS Kernel (CA-6):** Everything.

### 4. CA-6 Micro-OS Specific Audit: Starter Code, Bootloader & QEMU
A comprehensive recursive search across the repository confirms:
- **Rust Source Files (`.rs`):** **0 found**.
- **Cargo Manifests (`Cargo.toml`):** **0 found**.
- **Kernel Templates / Bootloaders:** **None provided**.
- **QEMU Configuration Scripts:** **None provided**.
- **Assessment Finding:** The repository contains **zero starter code for CA-6**. The student is expected to architect and construct the Rust Micro-OS from scratch or import a recognized educational template.

---

## 5. Deliverable 4: Challenge Bank & Allocation Status

The repository provides extensive scenario banks, but **contains no file, commit, or branch assigning specific challenges to any individual student**. 

In accordance with academic integrity and the prompt's strict rules, all unconfirmed assignments are categorized below and marked **`NEEDS FACULTY CONFIRMATION`**.

### Detailed Allocation Categorization

| CA | Allocation Status | Mandatory Tasks | Optional / Alternative Bank Choices | Action Required |
|---|---|---|---|---|
| **CA-1** | **NEEDS FACULTY CONFIRMATION** | Complete 5-stage analysis & 11-section report (§5–10). | Category A (A1–A2), B (B1–B4), C (C1–C4), D (D1–D3), E (E1–E3), F (F1–F3), G (G1–G3), H (H1–H3), I (I1–I3), J (J1–J4), Integrated (I1–I4). | Ask faculty if a specific scenario is assigned or if the student may pick from the bank. |
| **CA-2** | **NEEDS FACULTY CONFIRMATION** | Controlled experiment, 3+ workloads, 3+ repetitions, 18-section report. | Experiment 1 to 18 (e.g. Exp 1 CPU Scheduling, Exp 2 RR Quantum, Exp 5 Sync Contention, Exp 8 Memory, Exp 9 Page Replacement). | Confirm assigned experimental question with faculty. |
| **CA-3** | **NEEDS FACULTY CONFIRMATION** | Root cause diagnosis, fix implementation, 5-part test suite, regression evidence. | Category A through K (e.g. B1 Broken RR, C1 Broken Bank Account Race, D1 Circular Lock Deadlock, E1 Allocator Bug). | Confirm whether faculty provides buggy code or student injects faults into a bank topic. |
| **CA-4** | **NEEDS FACULTY CONFIRMATION** | Proposal, Literature Matrix (3–5 papers), 18-section research report. | Topics R1 to R32 (e.g. R2 Quantum Optimization, R19 Page Replacement for AI/ML access patterns). | **Mandatory Stage 4 Faculty Approval Checkpoint** (§22). Faculty must approve proposal. |
| **CA-5** | **NEEDS FACULTY CONFIRMATION** | Real Linux testing, baseline vs intervention, quantitative telemetry. | Challenge L1 to L43 (e.g. L1/L25 `/proc` explorer, L5 Priority renicing, L6 CPU affinity pinning). | Confirm chosen challenge with faculty. |
| **CA-6** | **NEEDS FACULTY CONFIRMATION** | Core 10-layer Rust kernel (Boot, Console, Tasks, Queue, RR, Timer, Lock, Allocator). | Choose 1 Specialization Track from Tracks A to G (§11) and 1 Variant from 20 variants (§12). | Clarify whether bare-metal QEMU is mandatory or user-space simulated kernel is acceptable; confirm specialization track. |
| **CA-7** | **MANDATORY** | Live artifact demonstration, 8–12 min oral defence, adaptive Q&A. | Choice of artifact to demonstrate (CA-6 Micro-OS or CA-5 Linux tool). | Await faculty viva schedule. |

---

## 6. Deliverable 5: Technical Feasibility, Windows & Rust Assessment, and Simplest Rubric Compliance Paths

### Evaluation Matrix for a 2nd-Year AI/ML Student on Windows

| CA | Difficulty (Beginner) | Estimated Time | Primary Tools & Software | Major Technical Risks | Simplest Genuine Implementation Path |
|---|:---:|:---:|---|---|---|
| **CA-1** | Low | 4–6 hrs | Markdown Editor, Python 3.14 (installed) | Superficial definition-dump without analytical model or trade-off evaluation. | Select **Challenge B1** (Interactive University Portal) or **C1** (Banking Race). Create clear queuing/state model, calculate response times for FCFS vs RR, and write the 11-section report. |
| **CA-2** | Medium | 6–8 hrs | Python 3.14, Matplotlib | Confounding variables, lack of repetitions, missing raw data. | Select **Experiment 2** (RR Time Quantum Investigation). Write pure Python discrete-event scheduler, test 6 quanta across 3 synthetic workloads (5 runs each), plot Quantum vs Response Time, and write the 18-section report. |
| **CA-3** | Medium | 5–7 hrs | Python 3.14 | Fixing symptoms without addressing root cause; breaking regression. | Select **Challenge C1** (Race condition on shared bank account). Demonstrate failing multi-threaded Python script, diagram thread race model, implement `threading.Lock` fix, run 5-part test suite, and present Before vs After evidence. |
| **CA-4** | Medium–High | 8–12 hrs | Python 3.14, Google Scholar / arXiv | Overly broad research scope; failing to meet 3–5 paper literature review minimum. | Select **Topic R19** (*Page Replacement for AI/ML-like Memory Access Patterns*). Compare FIFO, LRU, Optimal against sequential matrix sweeps vs random weights. Directly aligns with AI/ML background; requires only standard Python. |
| **CA-5** | High on Windows | 8–10 hrs | WSL 2 (Ubuntu), Bash, Python 3.x | **Windows Incompatibility**: `/proc`, `taskset`, `nice`, signals do not exist natively on Windows. Standard Windows sandbox blocks WSL. | Select **Challenge L1 / L25** (`/proc` Process Explorer & CPU Affinity). Execute inside WSL 2 (Ubuntu). Launch CPU-bound Python script, read `/proc/<pid>/stat`, apply `taskset` to bind core, measure execution speedup, and document before/after. |
| **CA-6** | **CRITICAL / EXTREME** | 25–40 hrs (from scratch) / 15–20 hrs (with template) | Rust toolchain, `cargo`, `rustup`, QEMU, Python | **Extreme Technical Risk**: Student is a Rust beginner. Zero starter code exists. Bare-metal `no_std` kernel development on Windows is notoriously complex and error-prone. | Adopt an established educational bare-metal Rust template (e.g. Philipp Oppermann's `blog_os` architecture or an approved minimal x86_64 bootloader). Implement simple cooperative Round Robin task queue, basic spinlock, and bump allocator. Specialization: Track A (Dynamic Quantum). Parse serial output in Python. |
| **CA-7** | Low–Medium | 4–6 hrs prep | Running QEMU / Python artifacts | Inability to answer live debugging/fault-injection questions; lack of familiarity with own code. | Prepare live demonstration of CA-6 Micro-OS in QEMU and CA-5 `/proc` tool; review the 7-level viva progression and pre-prepare answers to the CO Question Bank (§13–18). |

---

## 7. Deep-Dive: Platform & Environment Assessment

### Concrete Findings on Student Machine
1. **Python Setup**:
   - `python.exe` on default Windows PATH currently resolves to legacy `Python 2.7.11` (located in `C:\Program Files (x86)\MGLTools-1.5.7\python.exe`).
   - Modern `Python 3.14.7` is installed at `C:\Users\Vanshika\AppData\Local\Programs\Python\Python314\python.exe`.
   - **Urgent Action**: Environment PATH must be updated to prioritize Python 3.14, or all scripts must be executed using the full path / virtual environment.
2. **Rust & Cargo**:
   - `rustc` and `cargo` are **not installed** on Windows.
3. **QEMU Emulator**:
   - `qemu-system-x86_64` is **not installed** on Windows.
4. **Linux Environment (for CA-5)**:
   - Native Windows cannot run `/proc` exercises.
   - WSL must be configured with an active Ubuntu distribution, and CA-5 commands must be executed within the WSL Ubuntu shell.

---

## 8. Summary of What to Do First & Faculty Inquiries

### Phase 1: Immediate Student Actions (Today)
1. **Fix Python PATH:** Set Windows User PATH so `python` points to `Python 3.14` (`C:\Users\Vanshika\AppData\Local\Programs\Python\Python314\`).
2. **Install WSL 2 & Ubuntu:** Open administrative PowerShell and run `wsl --install -d Ubuntu` to ensure a working Linux environment for CA-5.
3. **Install Rust Toolchain:** Download and run `rustup-init.exe` from `rustup.rs` to install `rustc` and `cargo`.
4. **Install QEMU:** Install QEMU for Windows (via Chocolatey, winget `winget install SoftwareFreedomConservancy.QEMU`, or official installer) to enable CA-6 kernel emulation.

### Phase 2: Questions You Must Submit to Faculty
1. **Challenge Allocations (CA-1, CA-2, CA-3, CA-5):**
   > *"Are our challenges for CA-1, CA-2, CA-3, and CA-5 individually assigned by roll number, or are we permitted to select freely from the Challenge Banks in the Markdown files?"*
2. **CA-3 Defective Starter Code:**
   > *"Does faculty provide a buggy starter codebase for CA-3, or should we select a challenge from Category A–K and introduce/demonstrate the bug via fault injection?"*
3. **CA-4 Topic Approval Checkpoint:**
   > *"We propose Topic R19 ('Page Replacement for AI/ML-like Access Patterns') / Topic R2 ('Round Robin Quantum Optimization'). Can you approve this proposal for our CA-4 Checkpoint?"*
4. **CA-6 Micro-OS Scope & Template Approval:**
   > *"Since the repository does not contain starter code or bootloader templates for CA-6, which educational base template (e.g. Philipp Oppermann's blog_os / bootloader crate) does faculty approve for the minimal Rust kernel? Does faculty require bare-metal QEMU boot, or is a simulated user-space micro-kernel in Rust accepted?"*
5. **CA-6 Team vs Individual Policy:**
   > *"Is CA-6 evaluated as an individual project or a team project?"*

---
*End of Master Inspection Report. Maintain this document as the reference guide throughout implementation.*


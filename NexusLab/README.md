<div align="center">

# ⚡ NEXUS // ADVANCED PROGRAMMING LAB

### `A completely unnecessary amount of documentation for a university project.`

<img src="https://img.shields.io/badge/STATUS-ONLINE-00ff9d?style=for-the-badge&labelColor=0b0f14" alt="Status Online">
<img src="https://img.shields.io/badge/PYTHON-3.12-00d9ff?style=for-the-badge&logo=python&logoColor=white&labelColor=0b0f14" alt="Python">
<img src="https://img.shields.io/badge/OOP-100%25-bd00ff?style=for-the-badge&labelColor=0b0f14" alt="OOP">
<img src="https://img.shields.io/badge/COFFEE-∞-ff0055?style=for-the-badge&labelColor=0b0f14" alt="Coffee">

<br><br>

> **NEXUS** is a modular software experiment built for Advanced Programming.
> It combines object-oriented programming, data structures, algorithms and a suspicious
> amount of caffeine into one unnecessarily dramatic system.

</div>

---

## 🧬 PROJECT DNA

```text
                    ┌──────────────────────────────┐
                    │         N E X U S            │
                    │   ADVANCED PROGRAMMING       │
                    └──────────────┬───────────────┘
                                   │
             ┌─────────────────────┼─────────────────────┐
             ▼                     ▼                     ▼
       ┌───────────┐         ┌───────────┐         ┌───────────┐
       │  OBJECTS  │         │ ALGORITHMS│         │  DATA     │
       │   █████   │         │   █████   │         │ STRUCTURES │
       └─────┬─────┘         └─────┬─────┘         └─────┬─────┘
             │                     │                     │
             └─────────────────────┼─────────────────────┘
                                   ▼
                         ┌───────────────────┐
                         │   CHAOS CONTROL   │
                         │      ENABLED      │
                         └───────────────────┘
```

---

## 🎯 WHAT IS THIS?

NEXUS is a **fictional management and simulation platform** created as a project for a university course.

The system models entities, processes information, applies algorithms and generates useful results while demonstrating the core concepts expected from an Advanced Programming course.

### The mission

> Turn a bunch of classes, lists and functions into something that looks like a product that could launch a satellite.

---

## 🧠 CONCEPTS USED

| Concept | Implementation |
|---|---|
| 🧱 Classes | Domain entities |
| 🧬 Inheritance | Specialized entity types |
| 🔐 Encapsulation | Controlled attributes and methods |
| 🎭 Polymorphism | Different behaviors through common interfaces |
| 🧩 Abstraction | Separation of implementation and behavior |
| 🔄 Algorithms | Search, sorting and processing |
| 🗃️ Data Structures | Lists, dictionaries, queues, stacks |
| ⚠️ Exceptions | Controlled error handling |
| 💾 Persistence | Saving/loading application data |
| 🧪 Testing | Validation of critical components |

---

## 🗂️ ARCHITECTURE

```text
NEXUS/
│
├── 🚀 main.py
│
├── 🧠 core/
│   ├── models.py
│   ├── services.py
│   └── exceptions.py
│
├── ⚙️ algorithms/
│   ├── search.py
│   └── sorting.py
│
├── 💾 data/
│   ├── database.json
│   └── backup.json
│
├── 🧪 tests/
│   ├── test_models.py
│   ├── test_services.py
│   └── test_algorithms.py
│
├── 📚 docs/
│   └── architecture.md
│
└── 📄 README.md
```

---

## ⚙️ HOW THE MACHINE THINKS

```mermaid
flowchart LR
    A["👤 USER"] --> B["🖥️ INTERFACE"]
    B --> C["🧠 BUSINESS LOGIC"]
    C --> D["🧩 OBJECT MODEL"]
    D --> E["⚙️ ALGORITHMS"]
    E --> F["💾 DATA"]
    F --> G["📊 RESULT"]
    G --> B

    style A fill:#111827,stroke:#00ff9d,color:#fff
    style B fill:#111827,stroke:#00d9ff,color:#fff
    style C fill:#111827,stroke:#bd00ff,color:#fff
    style D fill:#111827,stroke:#ff0055,color:#fff
    style E fill:#111827,stroke:#ffe600,color:#fff
    style F fill:#111827,stroke:#00ff9d,color:#fff
    style G fill:#111827,stroke:#00d9ff,color:#fff
```

---

## 🛠️ INSTALLATION

### 01 — Clone

```bash
git clone https://github.com/usuario/nexus.git
cd nexus
```

### 02 — Create the environment

```bash
python -m venv .venv
```

### 03 — Activate it

**Windows**
```powershell
.venv\Scripts\activate
```

**Linux / macOS**
```bash
source .venv/bin/activate
```

### 04 — Install dependencies

```bash
pip install -r requirements.txt
```

### 05 — Launch NEXUS

```bash
python main.py
```

---

## 🎮 COMMAND CENTER

Once the program starts:

```text
╔══════════════════════════════════════╗
║          N E X U S   v1.0            ║
╠══════════════════════════════════════╣
║ [1] Create entity                    ║
║ [2] List entities                    ║
║ [3] Search                           ║
║ [4] Sort                             ║
║ [5] Execute process                  ║
║ [6] Statistics                       ║
║ [7] Save                             ║
║ [0] Shutdown                         ║
╚══════════════════════════════════════╝

SYSTEM STATUS: ████████████████████ 100%
CPU:           NORMAL
MEMORY:        STABLE
DEVELOPER:     QUESTIONABLE
```

---

## 🧪 EXAMPLE

```python
from nexus.core import EntityManager

manager = EntityManager()

manager.create(
    name="Atlas",
    category="experimental",
    priority=5
)

result = manager.search("Atlas")

print(result)
```

Output:

```text
╭────────────────────────────────────╮
│ ENTITY FOUND                        │
├────────────────────────────────────┤
│ ID       : 001                     │
│ NAME     : Atlas                   │
│ CATEGORY : experimental            │
│ PRIORITY : █████                   │
│ STATUS   : ACTIVE                  │
╰────────────────────────────────────╯
```

---

## 📈 ALGORITHMIC CORE

NEXUS intentionally demonstrates multiple approaches to common computational problems.

```text
SEARCH
 ├── Linear Search       O(n)
 └── Binary Search       O(log n)

SORTING
 ├── Bubble Sort         O(n²)
 ├── Selection Sort      O(n²)
 └── Python Sort         O(n log n)

DATA ACCESS
 ├── List                O(n)
 └── Dictionary          O(1) average
```

> The goal is not merely to make the program work.
> The goal is to understand **why** it works and what it costs computationally.

---

## 🧱 OBJECT-ORIENTED DESIGN

```text
                 ┌─────────────────┐
                 │     Entity      │
                 ├─────────────────┤
                 │ id              │
                 │ name            │
                 │ status          │
                 ├─────────────────┤
                 │ activate()     │
                 │ deactivate()   │
                 └────────┬────────┘
                          │
              ┌───────────┴───────────┐
              ▼                       ▼
      ┌───────────────┐       ┌───────────────┐
      │   Student     │       │    System     │
      ├───────────────┤       ├───────────────┤
      │ semester      │       │ version       │
      │ program       │       │ uptime        │
      └───────────────┘       └───────────────┘
```

This structure makes it possible to extend the project without rewriting its entire core.

---

## 🚨 ERROR HANDLING

Because software without error handling is just optimism:

```python
try:
    manager.process(entity)
except EntityNotFoundError:
    print("ERROR: Entity does not exist.")
except InvalidOperationError:
    print("ERROR: Operation not allowed.")
except Exception as error:
    print(f"CRITICAL: {error}")
```

---

## 🧪 TEST PROTOCOL

Run:

```bash
pytest
```

Expected:

```text
============================ test session ============================

tests/test_models.py       ✓
tests/test_services.py     ✓
tests/test_algorithms.py   ✓

========================= 100% PASSED ================================

SYSTEM INTEGRITY: NOMINAL
```

---

## 📊 PROJECT STATUS

```text
████████████████████████████████████ 100%

Architecture       ████████████████████ 100%
OOP                ████████████████████ 100%
Algorithms         ██████████████████░░  90%
Testing            ███████████████░░░░░  75%
Documentation      ███████████████████░  95%
Sleep              ██░░░░░░░░░░░░░░░░░░  10%
```

---

## 🧑‍💻 TEAM

| Role | Person |
|---|---|
| 🧠 Lead Developer | Your Name |
| 🧪 QA Engineer | Your Name |
| 🏗️ Architect | Your Name |
| ☕ Chief Coffee Officer | Your Name |

---

## 📜 DEVELOPMENT PHILOSOPHY

```text
          ┌───────────────────────────────────────┐
          │                                       │
          │   IF IT WORKS → UNDERSTAND IT         │
          │   IF IT BREAKS → DEBUG IT             │
          │   IF IT'S UGLY → REFACTOR IT          │
          │   IF IT'S PERFECT → CHECK AGAIN       │
          │                                       │
          └───────────────────────────────────────┘
```

### Golden rule

**Code is written for computers.  
Architecture is written for humans.**

---

## 🛰️ ROADMAP

- [x] Project foundation
- [x] Object model
- [x] Basic algorithms
- [x] Data structures
- [x] Exception handling
- [x] Persistence
- [ ] Automated deployment
- [ ] Graphical interface
- [ ] Distributed processing
- [ ] Artificial intelligence
- [ ] Conquer the university

---

## 📡 FINAL TRANSMISSION

```text
╔══════════════════════════════════════════════════════╗
║                                                      ║
║              N E X U S   O N L I N E                 ║
║                                                      ║
║       Built for Advanced Programming                 ║
║       Powered by Python                              ║
║       Fueled by deadlines                            ║
║                                                      ║
║              [ SYSTEM STABLE ]                       ║
║                                                      ║
╚══════════════════════════════════════════════════════╝
```

<div align="center">

### `Made with Python, questionable decisions, and too many comments.`

**⭐ Star the project if your professor gives it more than 3.0**

</div>

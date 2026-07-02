# AI & Human-Centric Red Teaming Framework
An enterprise-grade, locally isolated emulation framework designed to evaluate, baseline, and structurally defend Large Language Model (LLM) pipelines and Retrieval-Augmented Generation (RAG) architectures against high-impact threat vectors.

---

## 🏗️ Architecture Blueprint
├── modules/
│   ├── 01_human_risk/          # Pretexting & Social Engineering Emulation (ZPhisher)
│   ├── 02_infrastructure/      # Local Ollama & Llama 3.1 Environment Deployment
│   └── 03_adversarial_ai/      # Programmatic Exploit & Defense Engineering
│       ├── indirect_test.py    # Injection Baseline & Hardened Delimiter Scripts
│       └── rag_poison_test.py  # RAG Poisoning & Upstream Quarantine Pipeline
└── README.md
---

## 🚀 Core Components & Test Execution

### 1. Indirect Prompt Injection Baseline & Hardening
* **Module Pathway:** `modules/03_adversarial_ai/indirect_test.py`
* **Vulnerability Target:** Trust boundary confusion occurs when user-supplied, untrusted semantic data blends into an LLM's active token execution stream, allowing passive instructions to override administrative parameters.
* **Defense Mitigation:** Dynamic context encapsulation via isolated XML delimiter boundaries combined with deterministic, structural down-voting rules instructions.

```bash
# Execute the automated injection test suite
python3 modules/03_adversarial_ai/indirect_test.py

2. Retrieval-Augmented Generation (RAG) Poisoning & Active Quarantine
Module Pathway: modules/03_adversarial_ai/rag_poison_test.py

Vulnerability Target: Data supply chain contamination. Attackers strategically plant malicious instructions inside internal or public knowledge bases, forcing automated RAG ingestion tools to fetch payloads that compromise system availability or data integrity.

Defense Mitigation: An upstream regex-driven processing layer that proactively scans vector database returns and enforces string quarantines before content enters the model's context window.

# Execute the automated RAG poisoning simulation and defense pipeline
python3 modules/03_adversarial_ai/rag_poison_test.py

3. Human Risk Social Engineering Simulation
Module Pathway: modules/01_human_risk/

Infrastructure Target: Initial boundary ingress emulation utilizing automated phishing reverse-proxies to model credential harvesting and measure organizational human vectors.

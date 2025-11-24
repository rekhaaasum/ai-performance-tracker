# ai-performance-tracker
AI-powered agent built in Microsoft Copilot Studio to automate engineering performance evidence gathering.

### ✔ Continuous Feedback Support  
Managers can run the agent any time—weekly, monthly, or quarterly.

### ✔ Data Boundaries & Efficiency  
- Searches only the last **90 days** by default  
- Limits heavy retrieval  
- Prioritizes ADO PRs/work items for engineering responsibilities  

---

## 🎯 Problem Statement

Performance reviews often depend on incomplete recollection:

- Hard to recall examples from 6 months ago  
- Difficult to track contributions for high-activity engineers  
- Managers’ documentation styles vary  
- Evidence becomes subjective instead of objective  

The result:  
❌ Inconsistent reviews  
❌ Poor calibration  
❌ Bias toward recent memory  

The agent solves this by generating **objective, timestamped evidence** across systems.

---

## 💡 Solution Design

### **Input**
`TeamMemberName` (e.g., “John Smith”)

### **Core Workflow**
1. Read job responsibilities from a preloaded Excel template  
2. Retrieve signals for the given teammate  
3. Match signals to specific responsibilities  
4. Generate concise summaries  
5. Export as Excel or text  

### **Agent Instructions**
The system includes instructions for:

- Retrieval prioritization  
- PR/work item requirements  
- Data boundaries  
- Role-based filtering  
- Safe summarization  

---

## 🛠 Tech Stack & Concepts Used

- **Microsoft Copilot Studio**  
- **Retrieval-Augmented Generation (RAG)**  
- **M365 Graph Search**  
- **Azure DevOps Search Integration**  
- **OneDrive/SharePoint File Retrieval**  
- **LLM Prompt Engineering**  
- **Job Responsibility Mapping Logic**  
- **Structured LLM Output**  
- **Agent Design & Instruction Hierarchy**  

---

## 📈 Impact

### ⏱ 90% Reduction in Review Prep Time  
Replaced hours of manual digging with a 1-minute automated run.

### 🎯 Objective, Evidence-Based Reviews  
All examples include:

- PR numbers  
- Work item IDs  
- Timestamps  
- Direct links  

### 🤝 Adopted by Peer Managers  
Now used to support:

- Coaching conversations  
- Ongoing feedback  
- Quarterly checkpoints  
- Year-end reviews  

### 💬 Better Conversations  
Managers and engineers now enter review meetings on the same page—with real data.

---

## 📚 What I Learned

This project deepened my understanding of:

- AI agents in enterprise environments  
- Retrieval behavior and ranking  
- Instruction engineering & hierarchy  
- LLM reasoning with structured templates  
- Multi-source data fusion  
- Privacy-safe summarization  
- AI applied to people-management workflows  

This was a genuine “business problem meets AI solution” moment.

---

## 📎 Repository Contents (Recommended Structure)

Although this repo is primarily documentation-based, here is the recommended structure:

```
performance-tracking-ai-agent/
│
├── README.md # Full project explanation
├── system_instructions.txt # (Optional) Copilot Studio system prompt
├── job_responsibilities_template.xlsx # (Optional) Example template structure
├── screenshots/ # Screenshots of the agent in action
│ ├── agent_overview.png
│ ├── evidence_output.png
│ └── excel_template_example.png
└── diagrams/ # (Optional) Architecture or workflow diagrams
└── retrieval_workflow.png
```





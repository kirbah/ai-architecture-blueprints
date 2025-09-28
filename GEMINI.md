# AI Architecture Blueprints - Project Memo

This file stores key structural decisions and templates for the `ai-architecture-blueprints` project to ensure consistency.

---

### **GitHub Repository Structure**

The repository will follow this hierarchical structure. Each pattern gets its own numbered sub-directory.

```
/
|
├── patterns/
|   ├── 01-pattern-name/
|   |   ├── README.md                 <- The core explanation
|   |   ├── diagram-problem.svg         <- (Future) Exported SVG of the "before" state
|   |   ├── diagram-solution.svg        <- (Future) Exported SVG of the "after" state
|   |   └── diagram-source.excalidraw   <- (Future) Linkable source file
|
├── .gitignore
├── CONTRIBUTING.md
├── LICENSE
└── README.md
```

---

### **Pattern README.md Template**

Each pattern's `README.md` file should follow this template. The Mermaid code will be rendered automatically by GitHub.

````markdown
# [Pattern Number]. [Pattern Title]

**[Core Principle Statement]**

**Business Outcome:** [One-line statement framing the pattern in terms of business value (cost, revenue, risk).]

---

### The Problem

[Detailed description of the business/technical problem the pattern solves.]

### Real-World Consequences: [Section Title]

_(Note: This section is optional. Omit if strong, credible case studies cannot be found.)_

- **Case Study: [Title of Case Study]**
  - **The Incident:** [Brief, neutral description of what happened.]
  - **The Impact:** [Description of the business impact: financial, reputational, etc.]
  - **Source:** [Link to primary, high-quality source with a descriptive title.]
  - **Alternative source:** [Link to another high-quality source for corroboration.]

### The Architectural Solution

[Detailed description of how the pattern solves the problem.]

### Visual Blueprint

#### Problem State: [Problem State Title]

```mermaid
[Mermaid code for the "before" state]
```

#### Solution State: [Solution State Title]

```mermaid
[Mermaid code for the "after" state]
```

---

### Use This Pattern When...

- ...[Describe a specific business scenario, e.g., "your AI will interact directly with customers"].
- ...[Mention a key risk you are trying to mitigate, e.g., "the cost of an automated error is unacceptably high"].
- ...[List a specific organizational or technical constraint, e.g., "your knowledge is fragmented across multiple data silos"].
- ...[Connect to a strategic goal, e.g., "you need to demonstrate a clear productivity multiplier for a knowledge management project"].

---

### Trade-offs & Implementation Realities

- **Overhead for Simple Tasks:** This pattern can be overkill for simple, single-shot AI tasks. Applying it unnecessarily adds latency and complexity.
- **Planner Brittleness:** The quality of the entire outcome depends on the quality of the initial plan. A weak planning model can lead the system down the wrong path from the start.
- **[Another Trade-off]:** [Brief explanation of the trade-off.]
````

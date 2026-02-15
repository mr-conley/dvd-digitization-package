\# Week 05 CLI Prompt Log



\- \*\*Tool\*\*: Gemini CLI (v2.5)

\- \*\*Date\*\*: Feb 14, 2026



\## Activity 1: Mermaid Generation

\- \*\*Prompt\*\*: "Generate a Mermaid flowchart (flowchart TD) from SOP.md. Include explicit Start/End nodes and label every decision path. Save the output as diagrams/mermaid/process.mmd."

\- \*\*Validation\*\*: AI initially used `//` for comments. I manually refactored to `%%` and used the `-->|Label|` syntax to resolve Mermaid parser errors.



\## Activity 2: BPMN Generation

\- \*\*Prompt\*\*: "Read SOP.md and generate a BPMN 2.0 XML file. Use tasks for steps and gateways for decisions. Use lanes for 'IT Technician' and 'Software/Hardware'. Write to diagrams/bpmn/process.bpmn."

\- \*\*Human Refinement\*\*: Manually refactored lanes in bpmn.io to properly separate manual technician tasks from automated system encoding logic.


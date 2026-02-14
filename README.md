DVD Digitization for Archival Package

This repository contains the standardized documentation and logic models for converting physical DVD media into digital MP4 files.



📂 Repository Structure

This project follows "Docs-as-Code" principles, separating source files from exported artifacts:



SOP.md: The source-of-truth procedural document.



diagrams/mermaid/: Source (.mmd) and export (.png) for the process flowchart.



diagrams/bpmn/: Source (.bpmn) and export (.svg) for the BPMN collaboration model.



prompt-log/: Audit trail of AI CLI interactions used to generate these files.



🛠️ Reproduction Instructions

To regenerate the diagrams in this repository using the Gemini CLI, follow these steps:



Prerequisites

Node.js (v20+).



Gemini CLI installed globally: npm install -g @google/gemini-cli.



Generating the Mermaid Flowchart

Run the following command from the root directory to update the Mermaid source from the SOP:



Bash

gemini -p "Read SOP.md and generate a Mermaid flowchart (flowchart TD) including Start/End nodes and labeled decision paths. Write output to diagrams/mermaid/process.mmd."

Generating the BPMN XML

To generate the raw BPMN 2.0 XML code:



Bash

gemini -p "Read SOP.md and generate a BPMN 2.0 XML file with lanes for IT Technician and System. Write output to diagrams/bpmn/process.bpmn."

Note: The generated .bpmn file should be validated and refined in a visual editor like bpmn.io.



⚠️ Privacy \& Safety

This repository uses placeholders like \[CLIENT\_NAME] and \[SYSTEM\_NAME] to ensure no PII or sensitive system data is exposed in the CLI prompts or version history.



🏁 Final Steps for Submission

Save the file: Make sure it is saved as README.md in the root folder.



Commit the change: Run these in your terminal:



Bash

git add README.md

git commit -m "Add README with reproduction instructions for Gemini CLI"

Push to GitHub: If you've connected your repo, run git push origin main.


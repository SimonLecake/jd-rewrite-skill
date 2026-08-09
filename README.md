# jd-rewrite-skill
JD Evaluation Calibrator
An LLM-powered framework for improving AI resume screening accuracy through JD optimization, evaluation rubric design, and human-feedback-driven calibration.
1. Overview
AI resume evaluation systems often suffer from inconsistent decisions compared with human recruiters. This project explores optimizing Job Descriptions and evaluation criteria instead of modifying the underlying model.

Core idea: Treat the JD as an executable evaluation specification rather than a simple job advertisement.
2. Problem Statement
Traditional JDs are written for humans, while LLM-based screening systems may interpret requirements too literally.

Common issues:
• Preferred qualifications treated as mandatory.
• Example lists interpreted as exhaustive constraints.
• Experience requirements becoming absolute rejection rules.
• Non-traditional backgrounds being overlooked.
3. Solution Approach
Business JD
↓
Requirement Analysis
↓
Evaluation Rubric Design
↓
Weighted Scoring Rules
↓
AI Resume Evaluation Prompt
4. Supported Modes
Calibration Mode:
Input: JD + historical resumes + human evaluation results.
Workflow: analyze samples, extract hiring boundaries, design scoring rules, validate AI-human alignment.

JD Rewrite Mode:
Rewrite JDs into AI-friendly structures with explicit requirements, open-ended skills, bonus criteria and experience grading.
5. Core Design Principles
1. Preferred ≠ Mandatory
Preferred requirements should be treated as bonus criteria.

2. Examples ≠ Whitelists
Example lists should not restrict equivalent backgrounds.

3. Experience Should Be Graded
Direct, relevant and transferable experience should have different weights.

4. Human Feedback Drives Calibration
Historical human decisions provide evidence for improving AI reliability.
6. Workflow Architecture
JD
↓
Requirement Extraction
↓
Evaluation Rubric
↓
AI Screening Prompt
↓
Resume Evaluation
↓
Human Review Feedback
↓
Continuous Calibration
7. Output Artifacts
Generated artifacts include:
• Evaluation dimensions and scoring rules.
• Synonym and equivalent-experience rules.
• Misjudgment correction rules.
• Backtesting results.
• Web evaluation prompt templates.
8. Technology Stack
• Large Language Models (LLMs)
• Prompt Engineering
• Evaluation Framework Design
• Human Feedback Loop
• AI Quality Calibration
• RAG Extension
9. Why This Project Matters
Enterprise AI reliability is not only about model capability. Reliable AI adoption also requires evaluation standards, feedback loops and business-aligned instructions.
10. Repository Structure
jd-eval-calibrator/

├── README.md
├── docs/
│   ├── architecture.md
│   └── evaluation-framework.md
├── prompts/
│   ├── responsibility_prompt.md
│   └── requirement_prompt.md
├── examples/
│   └── sample_rubric.md
└── diagrams/
    └── workflow.png

# Automated Knowledge Artifact Creation: Using Multiple AI Tools to Explore Privacy and Data Protection in AI Systems

**Author:** Felipe Rezende Gardin (RA: 215766)  
**Institution:** Universidade Estadual de Campinas (UNICAMP), School of Electrical and Computer Engineering  
**Course:** IA382A — Human-AI Collaboration Seminar  
**Date:** June 2026  
**Instructor:** Neeli Prasad (IEEE Distinguished Lecture Series)

---

## Project Overview

This project demonstrates a practical methodology for creating comprehensive knowledge artifacts on AI ethics topics by orchestrating four complementary AI tools in sequence. Rather than writing a traditional essay, the project documents a transparent, reproducible pipeline that spans research, synthesis, refinement, and presentation.

The core topic is **Privacy and Data Protection in AI Systems**, motivated by Neeli Prasad's emphasis on privacy as a "cornerstone" that must be designed into AI systems from the start.

---

## The Four-Tool Pipeline

The project executes this workflow:

1. **Perplexity** (Research)  
   Gathers structured, cited information on AI privacy risks, regulatory frameworks (GDPR, EU AI Act), and real-world breach cases.

2. **Claude API** (Synthesis)  
   Analyzes seminar themes and research findings, synthesizing them into a coherent, well-structured technical article.

3. **QuillBot** (Refinement)  
   Explores how different writing styles (standard, formal, creative) affect clarity and accessibility of the same content.

4. **SlidesAI.io** (Presentation)  
   Automatically generates a professional slide deck for rapid dissemination of findings.

Each stage is fully documented with exact prompts, configurations, and outputs—following Prasad's emphasis on "disclosing your prompt engineering."

---

## Project Structure

```
ia382_final_project/
├── Main.tex                    # Main LaTeX document
├── Sections/
│   ├── CoverPage.tex          # Title page
│   ├── Abstract.tex           # Project abstract
│   ├── Introduction.tex       # Background and motivation
│   ├── Methodology.tex        # Detailed methodology for each tool
│   ├── Results.tex            # Tool outputs and comparative analysis
│   ├── Conclusions.tex        # Lessons learned and implications
│   └── References.bib         # Bibliography (GDPR, EU AI Act, differential privacy, etc.)
├── Main.pdf                   # Compiled PDF output
├── README.md                  # This file
└── img/                       # (Optional) Screenshots and figures
```

---

## Key Themes from Prasad's Seminar

- **Privacy as a cornerstone**: Privacy must be built in from day one, not added as an afterthought
- **Real-world harm**: Deepfake fraud (Hong Kong bank), health data blackmail, cyberbullying via AI-generated media
- **Regulatory momentum**: EU AI Act (2024) mirrors GDPR's emergence 10 years ago—a signal that AI privacy law is accelerating
- **Interdisciplinary collaboration**: Engineers, lawyers, ethicists, and social scientists must work together from the start
- **Transparency in AI tool use**: Students should "disclose your prompt engineering" and show their work as rigorously as mathematicians do

---

## How to Compile the PDF

**Requirements:**
- `pdflatex` (TeX Live or MiKTeX)
- `bibtex`
- Bash or similar shell

**Compile:**
```bash
cd /home/felipe/workspace/ia382_final_project
pdflatex Main.tex
bibtex Main
pdflatex Main.tex
pdflatex Main.tex
```

This generates `Main.pdf` with all sections, bibliography, and references.

---

## Key Outputs and Findings

### Research Phase (Perplexity)
- 15+ verified sources on AI privacy, GDPR, EU AI Act, differential privacy, federated learning
- Documented real-world cases: Hong Kong deepfake fraud, patient data leaks, cyberbullying

### Synthesis Phase (Claude API)
- 1800+ word comprehensive article on privacy in AI
- Sections: Why Privacy Matters, Real Harms, Regulatory Frameworks, Technical Safeguards, Governance & Human Oversight

### Refinement Phase (QuillBot)
- Three writing style variants (original, standard, formal) compared for clarity and accessibility
- Demonstrates how tone and vocabulary affect readability for different audiences

### Presentation Phase (SlidesAI.io)
- 9-slide deck covering all major topics
- Generated in ~12 minutes with no manual design intervention

### Comparative Analysis
| Tool | Quality | Time | Cost | Best For |
|------|---------|------|------|----------|
| Perplexity | 4/5 | 10–15 min | Free | Research foundation with citations |
| Claude API | 5/5 | 3–5 min | Free | Synthesis and technical depth |
| QuillBot | 3/5 | 8–10 min | Free (limited) | Style exploration and adaptation |
| SlidesAI.io | 3.5/5 | 10–15 min | Free (basic) | Rapid prototyping and dissemination |

**Total pipeline time:** ~45 minutes of active work. **Total cost:** $0.

---

## Lessons Learned

1. **Interdisciplinary Orchestration**: No single tool was sufficient. Value emerged from composing tools with different strengths, mirroring Prasad's call for engineers, lawyers, ethicists, and social scientists at the same table.

2. **Prompt Engineering as Discipline**: Documenting every prompt, configuration, and output enables reproducibility and trains practitioners to think critically about inputs and parameters that shape AI outputs.

3. **Human Judgment Remains Essential**: While tools accelerated content creation, humans made critical decisions at every stage: evaluating research quality, assessing synthesis accuracy, choosing style variants, and determining output readiness.

4. **Transparency Over Perfection**: Showing all work—including limitations and trade-offs of free-tier tools—better serves the goal of understanding human-AI collaboration than hiding the messy reality behind polished outputs.

---

## Extensions and Future Work

- **Additional tools**: Integrate Gemini (longer synthesis) or Canva (custom design) for comparative quality analysis
- **Longitudinal study**: Rerun the pipeline in 12 months to assess how AI capabilities and regulatory changes affect outputs
- **Peer review**: Have synthesized content reviewed by privacy experts for factual accuracy and completeness
- **Domain generalization**: Apply the pipeline to other seminar topics to demonstrate transferability

---

## Files and References

### Primary Sources
- **Prasad, N.** (2026). *Human-AI Collaboration: Ethics, Privacy, and Governance*. IEEE Distinguished Lecture, IA382A Seminar Series, UNICAMP.
- **European Union** (2024). *Regulation (EU) 2024/1689 — Artificial Intelligence Act*. Official Journal of the European Union.
- **European Union** (2016). *Regulation (EU) 2016/679 — General Data Protection Regulation (GDPR)*. Official Journal of the European Union.

### Technical References
- Dwork, C., & Roth, A. (2014). *The algorithmic foundations of differential privacy*. Foundations and Trends in Theoretical Computer Science, 9(3–4), 211–407.
- Cavoukian, A. (2009). *Privacy by Design: The 7 Foundational Principles*. Information and Privacy Commissioner of Ontario, Canada.
- Floridi, L., et al. (2019). *An ethical framework for a good AI society*. Minds and Machines, 29(4), 689–707.

---

## Contact & Attribution

**Author:** Felipe Rezende Gardin  
**Email:** gardinfelipe@gmail.com  
**Date:** June 21, 2026

This project was completed as a final assignment for IA382A (Human-AI Collaboration Seminar) at UNICAMP, directed by Prof. Neeli Prasad.

---

*Note: All tool outputs, prompts, and configurations are documented in full within `Sections/Methodology.tex` and `Sections/Results.tex` for reproducibility and transparency.*

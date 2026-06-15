# Benefits Navigator – USAII Global AI Hackathon 2026

**Track:** Undergraduate – Challenge 4: “Fix Systems People Depend On”  
**Live Demo:** [https://benefits-navigator-2026.netlify.app](https://benefits-navigator-2026.netlify.app)  
**GitHub Repo:** [https://github.com/shaheerrustam-ds/benefits-navigator-usaai](https://github.com/shaheerrustam-ds/benefits-navigator-usaai)

## Overview

Benefits Navigator is an AI-powered tool that helps individuals and families understand their potential eligibility for public benefits: **SNAP (food assistance), Medicaid, Housing Assistance, LIHEAP (utility bills), and Childcare Subsidy**. It translates complex government rules into plain language and provides actionable next steps – all while maintaining strict responsible AI principles.

## Key Features

- **Eligibility Check** – Household size, income, state, primary concern, optional notes.
- **Multi-Program Comparison** – Side-by-side cards showing likelihood, estimated benefits, key requirements, and next steps for all five programs.
- **Reasoning Trace** – Open by default, shows FPL threshold calculations, visual bars comparing income to program limits, confidence rationale, and explicit AI/human decision boundary.
- **Responsible AI** – “You may qualify” language, confidence badge, permanent disclaimer, 211 referral, “Flag for Human Review” with admin panel (`#flags`), and a dedicated Responsible AI summary box.
- **Stress Check** – Three‑question wellbeing check with empathetic AI response, grounding tips, and resources (988 Lifeline, 211).
- **Benefits Bingo** – Gamified 5×5 grid of eligibility factors; confetti on high‑likelihood programs.
- **DAO‑Style Community Resources** – Upvote/downvote real local resources for 12 states (CA, TX, FL, NY, IL, PA, OH, GA, MI, NC, AZ, WA) plus national fallback. Votes stored in localStorage.
- **Document Checklist** – Personalised checklist of required documents with checkboxes and PDF export (jsPDF).
- **Bilingual (EN/ES)** – Full UI translation, AI responses in selected language.
- **WCAG 2.1 AA Accessibility** – Skip link, aria labels, focus rings, keyboard navigation, high contrast.
- **Dark/Light Theme** – Toggle with localStorage persistence.
- **Self-Check** – Validates FPL math against 2026 federal poverty guidelines.

## Technologies Used

- HTML5, Tailwind CSS, JavaScript (ES2022)
- OpenRouter API (Gemini 2.0 Flash) – optional; graceful fallback to realistic mock data
- jsPDF, canvas-confetti
- LocalStorage for persistence (history, flags, votes, theme, language)
- Fonts: Space Grotesk, JetBrains Mono

## Responsible AI Statement

- **Risk:** An incorrect eligibility suggestion may cause false hope or missed benefits.
- **Mitigation:** Human‑review flag + 211 referral + all language uses “you may qualify” – never a guarantee.
- **Human‑in‑the‑loop:** A trained caseworker at your local agency (not this AI) decides final eligibility.

## How to Run Locally

1. Download `index.html`.
2. Open it in any modern browser (no server required).
3. For live AI responses, obtain a free Gemini API key from [aistudio.google.com](https://aistudio.google.com) and enter it in the banner – or simply use the built‑in demo mode (all features work with realistic mock data).

## Deployment

The app is a single static HTML file hosted on Netlify:  
[https://benefits-navigator-2026.netlify.app](https://benefits-navigator-2026.netlify.app)

## License

MIT License – see [LICENSE](LICENSE) (optional, you may add one).

## Contact

For questions or accessibility issues: [shaheerrustam@gmail.com](mailto:shaheerrustam@gmail.com)

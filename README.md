# AI-RESEARCH-ANALYZER
# 🔬 Research Analyzer: Advanced AI Assistant for Scientific Papers

[![Live Application](https://img.shields.io/badge/Launch-Research_Analyzer-blue?style=for-the-badge&logo=google-chrome)](https://researchanalyzer.kit62.com/)
[![Powered by Gemini](https://img.shields.io/badge/Powered_by-Gemini_AI_models-orange?style=for-the-badge)](https://aistudio.google.com/)

**Research Analyzer** is a free, client-side web application designed to accelerate literature reviews and scientific paper analysis. By leveraging the power of Google's Gemini AI, it transforms complex academic PDFs into interactive, structured, and easy-to-digest dashboards.

👉 **[Access the official tool here: researchanalyzer.kit62.com](https://researchanalyzer.kit62.com/)**

---

## 📑 Table of Contents
1. [What is Research Analyzer?](#what-is-research-analyzer)
2. [Live Interactive Demo](#live-interactive-demo)
3. [Key Features](#key-features)
4. [How to Get Your Free Gemini API Key](#how-to-get-your-free-gemini-api-key)
5. [How to Use the Tool](#how-to-use-the-tool)
6. [Frequently Asked Questions (FAQ)](#frequently-asked-questions-faq)
7. [Privacy & Security](#privacy--security)

---

## 🧠 What is Research Analyzer?
Reading and extracting valuable data from dense scientific papers (PDFs) is incredibly time-consuming. **Research Analyzer** acts as your Senior Scientific Assistant. You simply upload a paper, provide your own Gemini API Key, and the tool generates a comprehensive report locally in your browser.

It is built for researchers, PhD students, engineers, and academics who need to quickly extract methodologies, future research lines, and SWOT (Strengths, Weaknesses, Opportunities, Threats) analyses from literature.

---

## 🚀 Live Interactive Demo
Curious about what the output looks like? We have generated a sample report based on a hypothetical scientific paper to demonstrate the tool's capabilities. 

🔗 **[View the Interactive Demo Report Here](https://tu-usuario.github.io/research-analyzer/)** *(Nota para ti: Cambia este enlace por el de tu GitHub Pages cuando lo actives).*

In this demo, you can see the dynamic Mermaid diagrams, the LaTeX rendering for chemical and mathematical formulas, and the layout of the extracted insights.

---

## ✨ Key Features
* **Automated SWOT Analysis:** Instantly identifies the Strengths, Weaknesses, Opportunities, and Threats of the research in the paper for a deep and fast understanding.
* **Flowchart Generation:** Automatically reads the experimental methodology and generates **interactive diagrams** to visualize the logical flow.
* **Context-Aware AI Chat:** Ask direct questions about the uploaded paper. The AI strictly uses the document as its primary context and uses standard LaTeX for perfect mathematical and chemical rendering.
* **Future Research Lines:** Extracts both typical (incremental) and disruptive (innovative) future research directions suggested by the authors.
* **100% Client-Side Processing:** No databases. Your PDFs and data are processed entirely in your browser and sent directly to the Google Gemini API.
* **Exportable Standalone Reports:** Save your analysis as a fully functional, offline HTML file containing the AI kernel, so you can review the interactive chat and diagrams anywhere.
* * **Standalone Offline Reports (Shareable):** Don't waste your API quota re-analyzing the same paper. With a single click, you can export your entire current dashboard—including generated diagrams—into a single, lightweight, standalone HTML file. Save it locally to revisit your analysis offline, or attach it to an email to share your findings seamlessly with colleagues and co-authors.

---

## 🤖 The AI Persona: How the Chat Kernel Works
Unlike generic AI chatbots that often hallucinate or lose focus, Research Analyzer uses a highly tailored "Chat Kernel" with strict prompt engineering rules. We are fully transparent about how our AI is instructed to behave:

* **Profile & Tone:** The AI acts as a **Senior Scientific Assistant**. Its tone is strictly professional, academic, yet accessible, assuming the user has a technical background related to the uploaded document.
* **Strict Context-First Rule:** The AI is locked into the context of your uploaded paper. It will prioritize extracting answers *only* from the text provided, preventing it from bringing in outside biases initially.
* **AIGEK (AI General External Knowledge) Tagging:** If you ask a question that goes beyond the paper's scope, the AI is allowed to use its general knowledge to help you. However, it is mandated to strictly flag this external information using the **(AIGEK,)** mark and append a superscript footnote (e.g., `(AIGEK: AI General External Knowledge)`). This guarantees you always know what is in the paper versus what the AI added for context.
* **Smart Internal Citations:** Instead of hallucinating academic references, the AI is instructed to cite specific sections of the provided text. If you ask for the paper's original references, it will guide you to the DOI link.
* **Strict LaTeX Formatting:** The prompt forces the AI to output all mathematical equations, variables, and chemical formulas using standard double-escaped LaTeX. This ensures that our KaTeX engine renders everything flawlessly on your screen, from complex integrals to specific compounds like $\mathrm{Na}_2\mathrm{SiO}_3$.
* * **Bulletproof Diagrams via Strict JSON Schemas:** If you ask an LLM to write a diagram syntax directly, it will eventually break a parenthesis or an arrow, corrupting the entire flowchart. We engineered a bulletproof workaround. Research Analyzer forces the AI to extract the experimental methodology into a strict, predefined JSON schema (Nodes and Edges) with rich quantitative data. Our internal engine then safely translates this JSON payload into a beautiful, interactive, and zoomable Mermaid flowchart. Zero syntax errors, 100% reliability (or maybe 99% .

---

## 🔑 How to Get Your Free Gemini API Key
To keep this tool completely free and private, Research Analyzer uses a "Bring Your Own Key" (BYOK) model. Google provides generous free tiers for their Gemini AI.

Here is the exact step-by-step process to get your key in 2 minutes:

1. Go to **[Google AI Studio](https://aistudio.google.com/)** and log in with your standard Google account.
2. Look at the left sidebar and click on **"Get API key"**.
3. Click the blue button that says **"Create API key"**.
4. Select an existing Google Cloud project or let the system create a new one for you automatically.
5. A popup will appear with a long string of letters and numbers. **Copy this key**.
6. Go to **[Research Analyzer](https://researchanalyzer.kit62.com/)**, paste the key in the top input field, and you are ready to analyze!

*Note: The free tier currently allows up to 5 requests per minute and 20 per day. But that is for every project that you own. You can always create, for free, several projects with different api keys, which gives you, in practical terms, infinite free personal use.*

---

## 🛠️ How to Use the Tool
1. **Prepare:** Obtain your Gemini API Key as described above.
2. **Upload:** Go to [Research Analyzer](https://researchanalyzer.kit62.com/) and upload any scientific paper in PDF format.
3. **Analyze:** Click the "Analyze Document" button. The tool will parse the text and generate the dashboard.
4. **Interact:** Use the built-in chat to ask specific questions (e.g., *"What is the exact molar ratio used in step 2?"*).
5. **Export:** Click "Save Offline Report" to download the entire interactive session as a standalone HTML file.

---

## ❓ Frequently Asked Questions (FAQ)

**Is Research Analyzer completely free?** Yes! The web application is 100% free to use. You only need a Google Gemini API key, which Google currently provides for free under their AI Studio developer tier.

**Does the tool understand mathematical formulas and chemistry?** Absolutely. The AI is heavily prompt-engineered to output strict LaTeX formatting. The application uses KaTeX to perfectly render equations, sub-indices, and chemical compounds seamlessly in your browser.

**Can I use this on my mobile phone?** While the site is responsive, Research Analyzer is heavily optimized for desktop environments due to the dense nature of scientific dashboards, interactive charts, and PDF processing capabilities.

**Why did you build this?** As researchers, we were tired of generic AI chatbots forgetting the context of our PDFs or hallucinating data. We needed a structured, dashboard-style tool that forces the AI to extract specific metadata (like SWOT and Methodologies) without losing the ability to ask follow-up questions.

---

## 🛡️ Privacy & Security
Your privacy is paramount. **Research Analyzer does not have a backend database.** * We do not store your API keys.
* We do not store your PDFs.
* We do not read your chat logs.

When you upload a PDF, the text extraction happens locally in your browser. That text is then sent directly via HTTPS to Google's official Gemini API to generate the response. Once you close the tab, everything is gone unless you explicitly exported the report to your hard drive.

---

### 🌐 Ready to supercharge your literature review?
**[Start analyzing papers now at Research Analyzer](https://researchanalyzer.kit62.com/)**

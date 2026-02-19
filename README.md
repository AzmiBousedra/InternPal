# Intern Pal

> **I was tired of applying to internships manually, so AI did it for me.** A private automation suite designed to streamline the entire internship application lifecycle, from finding postings to submitting final packages.

<br>


![ezgif-330f5e5b94ef32cf](https://github.com/user-attachments/assets/d10a2bcc-cf27-436f-a892-8cf86ce0bf90)



<br>

## 💡 The Problem
The internship hunt is a numbers game that quickly becomes a full-time job. Manually searching portals, tailoring cover letters, and re-entering the same data for hundreds of applications is inefficient and error-prone. I wanted to engineer a solution to handle the repetitive heavy lifting so I could focus on interview prep and building my actual skills.

## 🚀 The Solution: Intern Pal v1.0
This is a modular CLI tool that automates the key stages of the application process. It can be run step-by-step or in a "Full Auto-Pilot" mode that chains all scripts together for an end-to-end, hands-free experience.

## 🛠️ Tech Stack
* **Core:** TypeScript, Node.js
* **Browser Automation & Scraping:** Playwright
* **AI & NLP:** Google Gemini 2.5 Flash API
* **Document Processing:** Docxtemplater, PizZip, LibreOffice-Convert
* **CLI UI/UX:** @inquirer/prompts, Chalk, Figlet, Gradient-String

## ⚙️ How It Works (The Pipeline)
Intern Pal is broken down into four distinct micro-scripts controlled by a master CLI dashboard:

1. **🔑 Session Management:** Uses Playwright's persistent contexts to log into the university job portal, handle 2FA securely, and save authentication cookies to disk to prevent repeated login flags.
2. **🕷️ Data Extraction (The Scraper):** Crawls the portal to extract job descriptions, company names, deadlines, and application routing data (Internal vs. External), saving them into dynamically generated local directories.
3. **🧠 AI Generation:** Feeds the scraped job descriptions into the Gemini API alongside a base set of personal instructions. The AI extracts key requirements and generates a highly targeted, job-specific cover letter. This data is injected into a DOCX template and asynchronously converted into a polished PDF.
4. **📦 Automated Packaging:** The browser takes over again, navigating deep into the portal's UI to upload the newly generated PDFs, bypass asynchronous UI loading states, and bundle them with my standard resume and transcript into a final "Application Package" ready for submission.

## 🔒 Why is this repository empty?
The source code for **Intern Pal** is hosted in a **private repository**.
Due to the powerful nature of automation tools and to prevent abuse of platform Terms of Service, the codebase is kept confidential. This repository serves as a portfolio showcase and architectural overview of the project.

**Created by Azmi-Salah Bousedra.**

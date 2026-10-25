# 🧠 OT Mental Health: 3-Week Study Tracker & RemNote Companion

[![GitHub Pages Deployment](https://img.shields.io/badge/GitHub%20Pages-Ready-success?logo=github)](https://pages.github.com/)
[![Curriculum](https://img.shields.io/badge/Curriculum-57%20Chapters%20(Complete)-indigo)](#curriculum-architecture)
[![Schedule](https://img.shields.io/badge/Pacing-3%20Weeks%20%7C%202--3%20hrs%2Fday-blue)](#3-week-schedule-overview)
[![Flashcards](https://img.shields.io/badge/Flashcards-RemNote%20Formatted-emerald)](#remnote-integration)
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](#license)

An interactive, responsive single-page web application designed to help occupational therapy students, practitioners, and licensure candidates systematically master **Brown, Stoffel, & Muñoz's *Occupational Therapy in Mental Health: A Vision for Participation* (2nd Edition)** over an intensive, manageable **3-week study schedule**.

---

## 🌟 Key Features

* **Complete 57-Chapter Coverage**: All 4 major parts mapped chronologically (Foundations, The Person, The Environment, Occupation) across pages 3–940.
* **Balanced 21-Day Schedule**:
  * **18 Active Study Days**: ~3 chapters per day (45–60 pages of reading + AI flashcard drafting = 2–3 hours daily).
  * **3 Dedicated Review Days** (Days 7, 14, 21): Spaced-repetition card drills, diagnostic comparison matrices, and PEO case synthesis.
* **AI-Assisted RemNote Flashcard Engine**:
  * **Pre-Built Decks**: Every chapter features ready-to-copy RemNote cards formatted with concepts (`::`), two-way reversibles (`==`), clozes (`[...]`), and multi-line structures (`:::`) covering DSM-5 diagnostic criteria, assessment tools, and OT interventions.
  * **1-Click Copy**: Instant clipboard copy for each chapter's deck or bulk export across all 57 chapters.
  * **Custom AI Prompt**: Ready-to-use LLM prompts pre-populated with chapter titles, subtopics, and page numbers for generating custom deep-dive cards.
* **Interactive Tracking & Persistence**:
  * **LocalStorage Auto-Save**: All checkmarks, chapter statuses (`⚪ Not Started`, `🟡 Reading In Progress`, `🔵 Cards Drafted`, `🟢 Mastered`), personal notes, and timers persist across browser refreshes.
  * **Granular Subtopic Checklists**: Interactive checkboxes for every subsection extracted directly from the book's Table of Contents (pages 24–37).
  * **Built-In Pomodoro Focus Timer**: 25m Focus / 50m Deep / 5m Break modes with audio alerts.
  * **Dynamic Real-Time Filters & Search**: Instant client-side search across chapter titles, DSM diagnoses, assessment tools (*COPM*, *ACLS*, *Sensory Profile*), and models.
* **Clinical Toolboxes (Appendices A–D)**:
  * **Appendix B**: Searchable Index of 150+ Standardized Assessments with 1-click links to corresponding chapters.
  * **Appendix C**: Searchable Index of Evidence-Based OT Interventions with targets and synopses.
  * **Appendix D**: Practice Models & Theoretical Frameworks (PEO, MOHO, EHP, Kawa, Recovery Framework).
* **Backup & Restore**: Export your progress as a JSON snapshot to save or transfer across devices.
* **Zero Dependencies**: 100% self-contained HTML/CSS/JS that works offline and is fully ready for GitHub Pages!

---

## 🚀 GitHub Pages Deployment Guide

Deploying this site to GitHub Pages takes under 2 minutes:

### Method 1: Push This Folder to a New GitHub Repository

1. Open your terminal in this folder:
   ```bash
   cd "C:\Users\James Ong\Documents\antigravity\self-learning\Study Tracker"
   ```
2. Initialize git and commit:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: OT Mental Health 3-Week Study Tracker"
   ```
3. Create a new repository on [GitHub](https://github.com/new) (e.g. `ot-mental-health-study-tracker`).
4. Link the remote and push:
   ```bash
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo-name>.git
   git push -u origin main
   ```
5. On GitHub, navigate to **Settings** > **Pages** (under "Code and automation"):
   * Under **Build and deployment** > **Source**, choose **Deploy from a branch**.
   * Under **Branch**, select **`main`** and **`/(root)`**, then click **Save**.
6. Within 1–2 minutes, your website will be live at:
   ```
   https://<your-username>.github.io/<your-repo-name>/
   ```

*(Note: The included `.nojekyll` file ensures that GitHub Pages serves all static files directly without Jekyll filtering).*

---

### Method 2: Offline / Local Use

Double-click `index.html` in Windows File Explorer or open it in any browser:
```powershell
Start-Process "index.html"
```
No web server, Node.js, or external Internet connection is required.

---

## 📅 3-Week Schedule Overview

```
WEEK 1: Foundations & Diagnoses (Days 1–7)
├─ Day 1: Ch 1 (Recovery), Ch 2 (OT History), Ch 3 (PEO Model)
├─ Day 2: Ch 4 (Evaluation), Ch 5 (Evidence-Based Practice), Ch 6 (Intro to The Person)
├─ Day 3: Ch 7 (Autism), Ch 8 (Intellectual Disabilities), Ch 9 (ADHD)
├─ Day 4: Ch 10 (Conduct/Disruptive), Ch 11 (Eating Disorders), Ch 12 (Personality Disorders)
├─ Day 5: Ch 13 (Mood Disorders), Ch 14 (Anxiety/OCD), Ch 15 (Trauma & Stressor-Related)
├─ Day 6: Ch 16 (Schizophrenia), Ch 17 (Substance & Co-Occurring), Ch 18 (Dementia), Ch 19 (Physical Disabilities)
└─ Day 7: 🔄 Week 1 Consolidation, Spaced-Repetition Drill & PEO Clinical Synthesis (Ch 1–19)

WEEK 2: Performance Skills & The Environment (Days 8–14)
├─ Day 8: Ch 20 (Cognition), Ch 21 (Cognitive Beliefs), Ch 22 (Sensory Processing)
├─ Day 9: Ch 23 (Coping & Resilience), Ch 24 (Motivation), Ch 25 (Emotion)
├─ Day 10: Ch 26 (Communication & Social Skills), Ch 27 (Pain), Ch 28 (Time Use & Habits)
├─ Day 11: Ch 29 (Intro to Environment), Ch 30 (Public Policy), Ch 31 (Stigma & Recovery)
├─ Day 12: Ch 32 (Families), Ch 33 (Sociocultural Perspectives), Ch 34 (Community), Ch 35 (Supportive Housing)
├─ Day 13: Ch 36 (Early Intervention), Ch 37 (Early Psychosis), Ch 38 (Peer-Led Services), Ch 39 (Criminal Justice)
└─ Day 14: 🔄 Week 2 Consolidation, Spaced-Repetition Drill & Environmental Synthesis (Ch 20–39)

WEEK 3: Practice Settings & Occupations (Days 15–21)
├─ Day 15: Ch 40 (State Hospitals), Ch 41 (Crisis Continuum & ACT), Ch 42 (Shelters)
├─ Day 16: Ch 43 (Wraparound), Ch 44 (Veterans & Military), Ch 45 (Primary Care), Ch 46 (Entrepreneurial Skills)
├─ Day 17: Ch 47 (Intro to Occupation), Ch 48 (Wellness), Ch 49 (ADLs & IADLs)
├─ Day 18: Ch 50 (School Mental Health), Ch 51 (Adult Education), Ch 52 (Work), Ch 53 (Volunteering)
├─ Day 19: Ch 54 (Social Participation), Ch 55 (Leisure & Play), Ch 56 (Rest & Sleep), Ch 57 (Spiritual Occupation)
├─ Day 20: 🛠 Appendices Deep-Dive: PEO Analysis, Assessments (App B), Interventions (App C), Models (App D)
└─ Day 21: 🏆 Final Cumulative Mastery & Comprehensive RemNote Spaced-Repetition Drill (All 57 Chapters)
```

---

## 🗂 File Structure

```
Study Tracker/
├── index.html                   # Main interactive web app (self-contained)
├── ot_study_master_data.json    # Complete JSON dataset of chapters, assessments, and models
├── favicon.svg                  # Vector brain favicon for browser tabs
├── .nojekyll                    # Tells GitHub Pages not to run Jekyll build
├── .gitignore                   # Ignores OS and temporary cache files
├── README.md                    # Project documentation & GitHub Pages deployment guide
└── scripts/                     # Python data-processing and site-generation tools
    ├── build_html_website.py
    ├── generate_master_data.py
    ├── chapter_content_generator.py
    ├── chapter_content_specialized.py
    ├── map_appendices.py
    └── parse_toc.py
```

---

## 📝 RemNote Flashcard Syntax Guide

The pre-built flashcard decks use native RemNote markdown formatting for instant paste:

* **Concept Card (`::`)**:
  ```markdown
  Recovery (SAMHSA Definition):: A process of change through which individuals improve their health and wellness, live a self-directed life, and strive to reach their full potential.
  ```
* **Two-Way Reversible Card (`==`)**:
  ```markdown
  Clinical Recovery vs Personal Recovery == Clinical recovery focuses on symptom reduction and cure; Personal recovery focuses on meaning, empowerment, and living well with mental illness.
  ```
* **Cloze Deletion (`[...]`)**:
  ```markdown
  The Duration of Untreated Psychosis (DUP) is the interval between [first psychotic symptoms] and [initiation of treatment].
  ```
* **Multi-Line List Card (`:::`)**:
  ```markdown
  SAMHSA 4 Dimensions of Recovery :::
  - **Health**:: Overcoming or managing symptoms and making informed healthy choices.
  - **Home**:: Having a stable and safe place to live.
  - **Purpose**:: Meaningful daily activities and independence.
  - **Community**:: Relationships and social networks providing support and hope.
  ```

---

## 📄 License & Attribution

* Content based on: *Occupational Therapy in Mental Health: A Vision for Participation* (2nd Edition) by Catana Brown, Virginia C. Stoffel, & Jaime Phillip Muñoz (F.A. Davis).
* Study Tracker application code licensed under the [MIT License](LICENSE).

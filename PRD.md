# Product Requirement Document (PRD): Vibe Coding Portfolio

**Project Name:** Vibe Coding - Academic Portfolio Refactor
**Base Repository:** [academicpages.github.io](https://github.com/academicpages/academicpages.github.io)
**Local Path:** `Desktop/Hackathon`
**Author:** Stephan Ihm
**Date:** December 15, 2025
**Status:** In Progress

---

## 1. Project Overview
The goal is the transformation of the "Academic Pages" template into a highly personalized portfolio ("Vibe Coding"). The focus is on aesthetics, personal branding, and the clean transfer of academic content into a modern web format.

---

## 2. Technical Constraints & Environment
* **Framework:** Jekyll (Ruby Static Site Generator).
* **Hosting:** GitHub Pages.
* **Data Source & Assets:** Specific instructions and source files are located in the `custom assets/` folder.
* **Constraints:**
    * **Frameworks:** No new CSS/JS frameworks (maintain existing Bootstrap version, no Tailwind/React).
    * **JavaScript:** Vanilla JS is permitted for UI logic (e.g., Dark Mode Toggle); external libraries are to be avoided.
    * **Code Style:** Modifications primarily in `_layouts`, `_includes`, `_sass`, and Markdown content.

---

## 3. Milestones

### Milestone 1: Theme Customization & Dark Mode
**Goal:** Implementation of a user-controlled theme switch (Light/Dark), as the template natively supports this only partially or statically.

* **Requirement:** Add a toggle button to the main navigation (`_includes/masthead.html`).
* **Tech Stack:** Vanilla JavaScript + CSS/SCSS.
* **Behavior:**
    * Click toggles a class on the `<body>` (e.g., `.dark-theme`).
    * State is saved in `localStorage` (Persistence on reload).
    * Verification of SCSS variables to ensure readability in both modes.

### Milestone 2: Homepage Customization
**Goal:** Construction of the landing page (`index.html` / `index.md`) according to specific layout guidelines.

* **Input Source:** `custom assets/layout_instructions.md` (file located in project folder).
* **Implementation:**
    * Analysis of the layout instructions.
    * Adaptation of the Frontmatter and HTML structure of the homepage.
    * Integration of "Vibe" elements (imagery, tonality) according to specifications.

### Milestone 3: CV Transformation
**Goal:** Transfer of the PDF CV into a responsive, structured web presentation.

* **Input Source:** `custom assets/Stephan Ihm_CV.pdf`.
* **Data Structure:**
    * Extraction of content (Experience, Education, Skills).
    * Transfer into YAML files (`_data/experience.yml`, `_data/education.yml`, etc.) for clean separation of content and design.
* **Frontend:**
    * Creation of a `cv.md` (or utilization of the existing one) that iterates and renders these YAML data.
    * Chronological timeline view.

### Milestone 4: Project Showcase
**Goal:** Creation of an interactive detail page for a selected portfolio case.

* **Features:**
    * Interactive elements (e.g., hover states, collapsible details, minor CSS animations).
    * Focus on storytelling (Problem -> Solution -> Result).
* **Integration:** Link in the main navigation.

---

## 4. Asset Management
* All project-specific raw data (PDFs, instructions) remain in the `custom assets/` folder to keep the repository clean.
* Images for the website will be transferred to `images/` or `assets/images/`.

---

## 5. Definition of Done
A milestone is considered complete when:
1.  The code builds locally (`jekyll serve`) without errors.
2.  The requirements are visually implemented.
3.  The changes are committed to Git.
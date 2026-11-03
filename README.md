# NMKHDL Project 09 – arXiv Data Pipeline

**Course:** Introduction to Data Science  
**Institution:** Ho Chi Minh City University of Science (HCMUS)  
**Student ID:** 24127061  
**Project:** Group 09

## 1. Project Overview

This repository contains the project report for the arXiv Data Pipeline developed as part of the Introduction to Data Science course at HCMUS.

The project focuses on collecting, processing, and organizing arXiv research papers to construct a structured dataset for subsequent analysis.

The report documents the implementation, methodology, experimental results, and performance evaluation across the project milestones.

## 2. Project Milestones

### Milestone 1 – Data Crawling

**Status: Completed**

This milestone focuses on building the data crawling pipeline to collect arXiv research papers and their associated information.

Main tasks include:

- Discovering papers within the assigned arXiv ID range.
- Identifying and downloading available paper versions.
- Collecting full-text LaTeX source files.
- Processing source archives and removing binary figure files.
- Collecting bibliographic metadata through arXiv OAI-PMH.
- Retrieving reference metadata through Semantic Scholar.
- Evaluating crawling performance and organizing the resulting corpus.

### Milestone 2 – Hierarchical Parsing and Standardization

**Status: Upcoming**

This milestone focuses on processing the collected LaTeX documents and transforming them into standardized hierarchical representations.

Main tasks include:

- Parsing LaTeX documents.
- Constructing hierarchical document structures.
- Standardizing extracted elements.
- Deduplicating document information.
- Extracting references into a unified BibTeX representation.

## 3. Project Report

The report is organized as a Jupyter Book and published using GitHub Pages.

**Access the online report:**

[Milestones 1–2 | arXiv Data Pipeline](https://khoabautroi.github.io/NMKHDL_G09_report/)

The report will be updated as subsequent project milestones are completed.

## 4. Technology Stack

The project uses the following technologies and services:

| Technology | Purpose |
|---|---|
| Python | Data collection and processing |
| arXiv API | Paper discovery |
| arXiv OAI-PMH | Bibliographic metadata collection |
| Semantic Scholar API | Reference metadata retrieval |
| LaTeX | Research paper source format |
| Jupyter Book | Report generation |
| Sphinx | Documentation build system |
| Mermaid | Pipeline workflow visualization |
| Git and GitHub | Version control and source hosting |
| GitHub Actions | Automated report deployment |
| GitHub Pages | Online report hosting |

## 5. Repository Structure

```text
NMKHDL_G09_report/
│
├── .github/
│   └── workflows/
│       └── deploy.yml
│
├── milestone1/
│   └── milestone1.md
│
├── index.md
├── _config.yml
├── _toc.yml
├── requirements.txt
├── .gitignore
└── README.md
```

## 6. Building the Report Locally

To build the Jupyter Book locally, follow these steps.

### 6.1 Create a Virtual Environment

```bash
python -m venv .venv
```

Activate the environment on Windows:

```powershell
.venv\Scripts\Activate.ps1
```

### 6.2 Install Dependencies

```bash
pip install -r requirements.txt
```

### 6.3 Build the Jupyter Book

```bash
jupyter-book build .
```

The generated HTML website will be available in:

```text
_build/html/
```

Open `_build/html/index.html` in a browser to view the report locally.

## 7. Deployment

The report is automatically built and deployed to GitHub Pages using GitHub Actions.

Whenever changes are pushed to the `24127061` branch, the deployment workflow runs automatically.

Published website:

https://khoabautroi.github.io/NMKHDL_G09_report/

## 8. License and Academic Purpose

This repository is maintained for academic purposes as part of the Introduction to Data Science course at HCMUS.

It documents the development and evaluation of the arXiv Data Pipeline project.

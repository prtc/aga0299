# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

This repository contains course materials for astrophysics education at Universidade de São Paulo. The project focuses on creating lecture content about working with astronomical data, following a systematic workflow for academic content development.

## Content Development Workflow

### Primary Format
- **Quarto documents** (.qmd) are the primary format for all lecture content
- **Multiple output targets**: RevealJS presentations, HTML course pages, PDF when needed
- **Academic publishing standards** with proper citation management and cross-referencing

### Development Process
1. **Conceptual discussion** → outline and structure planning
2. **Content creation** → direct .qmd file writing using file system tools
3. **Technical integration** → code examples, visualizations, interactive elements
4. **Quality assurance** → accuracy verification, technical testing, accessibility review

### Common Commands
- `quarto render` - Render all Quarto documents
- `quarto preview` - Live preview during development
- `quarto render file.qmd --to revealjs` - Render specific presentation
- `quarto render file.qmd --to html` - Render as HTML course page

## Content Standards

### Academic Requirements
- **Accurate attribution** for all sources and references
- **BibTeX integration** for citation management
- **Cross-referencing** for figures, tables, equations
- **Multiple representations** (verbal, visual, mathematical, computational)

### Technical Specifications
- **R code integration** using native pipe `|>` (not magrittr `%>%`)
- **Modern tidyverse practices** (pivot_longer/wider, mutate(across()), etc.)
- **Explicit namespace calls** for clarity (e.g., `readr::read_csv()`)
- **RevealJS customization** for professional academic presentations

### Quarto/Markdown Formatting Rules
- **CRITICAL**: Always add an empty line before bullet lists or numbered lists
- Without the empty line, lists will not render properly in RevealJS presentations
- This applies to all list structures within slide content

### Quality Assurance
- **Factual accuracy** verification for astronomical content
- **Mathematical correctness** for equations and calculations
- **Code functionality** testing for embedded examples
- **Multi-platform compatibility** (Windows, Mac, Linux)
- **Mobile responsiveness** for student access

## Repository Structure

### Content Organization
- **arXiv-1905.13189v2/** - Source materials and figures from "A Beginner's Guide to Working with Astronomical Data"
- **lecture_prep_workflow.md** - Detailed workflow documentation and guidelines
- **Images and figures** - Astronomical visualizations, plots, and educational diagrams

### File Types
- **LaTeX source** (.tex) - Original academic paper content
- **Image assets** - Astronomical data visualizations (.pdf, .jpg, .png)
- **Educational figures** - Diagrams for concepts like photometry, spectroscopy, data analysis

## Content Focus Areas

The materials cover fundamental astronomical data analysis topics:
- **Image data** processing and analysis techniques
- **Spectroscopic data** handling and interpretation
- **Catalog data** management and statistical analysis
- **Data cubes** and multi-dimensional datasets
- **Modern survey data** and database operations
- **Simulation data** from N-body and grid-based models

## Collaboration Model

### Content Authority
- Subject matter expertise from established astronomical research
- Pedagogical decisions based on university course requirements
- Technical implementation following modern academic publishing practices

### Development Priorities
- **Efficiency** through systematic workflow and reusable components
- **Reproducibility** with version control and documented processes
- **Accessibility** for diverse student backgrounds and needs
- **Professional quality** matching academic publication standards
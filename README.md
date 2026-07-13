# Liberal Arts

A collection of interactive, browser-based educational modules for foundational liberal arts subjects, including logic, mathematics, and statistics.

[🚀 Open Launcher](https://chess-r-quarto.github.io/liberal_arts/navi.html)

## Overview

This repository contains single-file web applications designed to aid in the learning and reference of various academic concepts. Each module is built using React and TypeScript, running entirely in the browser without the need for a local Node.js build environment.

## Modules

- **Launcher** (`navi.html`): An Anaconda Navigator-style dashboard that provides easy access to all the modules in this repository.
- **Logic Basic** (`logic_basic.html`): Covers the fundamentals of logic, including propositional and predicate logic.
- **Logic Terminology** (`logic_term.html`): Covers important terms and concepts in logic and set theory.
- **Math Terminology** (`math_term.html`): A comprehensive reference and explanation of basic mathematical terms across algebra, analysis, and geometry.
- **Stat Terminology 1** (`stat_term.html`): Focuses on descriptive statistics and foundational probability concepts.
- **Stat Terminology 2** (`stat_term2.html`): Covers inferential statistics, hypothesis testing, and regression analysis.

## Usage

All applications in this repository are completely self-contained. To use them:

1. Clone or download this repository to your local machine.
2. Open `navi.html` (or any individual module file) directly in any modern web browser.

*No Node.js, `npm install`, or build steps are required.*

## Architecture

These applications follow a strict single-file architecture:

- **Framework**: React (loaded via CDN)
- **Styling**: Tailwind CSS (loaded via CDN)
- **Language**: TypeScript (TSX) compiled in-browser using `@babel/standalone`

## CI/CD

Automated workflows are managed via GitHub Actions located in the `.github/workflows` directory.

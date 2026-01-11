---
inclusion: always
---
# Mission: Resume-as-Code

## Purpose

This repository implements a "resume-as-code" system where:
- Resume content is stored as reusable, atomic Markdown files
- Tailored resumes are assembled programmatically from these atoms
- All assembly logic lives in steering files, not scripts
- Kiro IDE handles the orchestration through natural language prompts

## Definition of Resume-as-Code

Resume-as-code means treating your professional history like source code:
- **Atomic content**: Each role, project, achievement, skill exists as a separate file
- **Version controlled**: All changes tracked in git
- **Reusable**: Content atoms can be mixed and matched for different opportunities
- **Consistent**: Standardized formats ensure quality and ATS compatibility
- **Maintainable**: Updates to atoms automatically improve all resumes that use them

## Core Principles

1. **Truth in one place**: Each fact exists in exactly one file
2. **No fabrication**: Missing information is marked with TODO, never invented
3. **Universal applicability**: Works for any profession, not just engineering
4. **Markdown-only**: No scripts, templates, or complex tooling
5. **Steering-driven**: All behavior defined in .kiro/steering/ files

## Non-Goals

- This is NOT a resume template system
- This is NOT a job application tracker
- This is NOT a portfolio website generator
- This does NOT generate cover letters or other documents
- This does NOT integrate with job boards or ATS systems directly

## Guardrails

- Never invent facts, experiences, or metrics
- Always mark missing information with TODO markers
- Maintain professional tone and accuracy
- Respect privacy and confidentiality of past employers
- Follow industry standards for resume formatting
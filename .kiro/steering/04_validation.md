---
inclusion: always
---

# Resume Validation and Quality Assurance

## Purpose
This file defines the validation process that Kiro must perform on every generated resume to ensure compliance with all steering files and quality standards.

## Mandatory Validation Process
Before finalizing any resume, Kiro MUST validate against ALL steering files in sequential order:

### 1. Mission Compliance (00_mission.md)
- [ ] **Truth in one place**: All content sourced from profile/experience files only
- [ ] **No fabrication**: No invented facts, experiences, or metrics
- [ ] **Markdown-only**: Clean markdown format with no scripts or complex tooling
- [ ] **Professional accuracy**: All company names, dates, and titles are exact
- [ ] **TODO-free**: No TODO markers remain in final output

### 2. Repository Structure Compliance (01_repo_map.md)
- [ ] **Content sourcing**: All content properly sourced from designated files
- [ ] **File relationships**: Profile files included, experience files selectively used
- [ ] **Naming convention**: Output file follows `{target-role}-{date}.md` format

### 3. Content Model Compliance (02_content_model.md)
- [ ] **Profile integration**: All profile files (identity, summary, skills, education, certifications) included
- [ ] **Experience selection**: Content properly selected from roles.md and projects.md
- [ ] **Structured format**: Content follows defined patterns and frontmatter standards

### 4. Harvard Writing Standards Compliance (03_writing_rules.md)
- [ ] **Section order**: Follows Harvard standard (Header → Education → Experience → Projects → Skills → Certifications)
- [ ] **Bullet format**: All bullets are one line maximum
- [ ] **Header format**: Includes name, contact, LinkedIn/portfolio in proper format
- [ ] **Action verbs**: Uses Harvard-approved strong action verbs (Led, Developed, Implemented, etc.)
- [ ] **CAR format**: Bullets follow Context + Action + Result structure
- [ ] **Quantification**: All achievements include specific metrics and percentages
- [ ] **Active voice**: Consistent active voice throughout ("Led team of 5" not passive voice)
- [ ] **No pronouns**: Avoids I, me, my, we, us throughout
- [ ] **Parallel structure**: Consistent verb tenses and formats within sections
- [ ] **Maximum bullets**: No more than 4 bullets per role
- [ ] **Length compliance**: Meets Harvard length guidelines (1 page for 0-5 years, 2 pages max for 5+ years)

### 5. Assembly Rules Compliance (05_resume_assembly_rules.md)
- [ ] **Content selection**: Prioritizes recent experience (last 5-10 years)
- [ ] **Relevance scoring**: Selected content matches target role requirements
- [ ] **Impact prioritization**: Emphasizes quantified achievements
- [ ] **Mandatory inclusions**: All profile files included, current role included
- [ ] **Proper ordering**: Reverse chronological for roles, impact-based for projects
- [ ] **Length constraints**: Meets target length for experience level
- [ ] **Metadata inclusion**: Proper generation metadata at top of file

### 6. Template Compliance (06_template.md)
- [ ] **Role adaptation**: Content properly adapted for target role and industry
- [ ] **Section configuration**: Follows Harvard standard section order
- [ ] **Industry terminology**: Uses appropriate terminology for target industry
- [ ] **Technical depth**: Matches appropriate level for target audience
- [ ] **Bullet allocation**: Follows Harvard bullet allocation standards
- [ ] **Quality checklist**: Passes all template quality assurance checks

## Validation Failure Protocol
If ANY validation check fails, Kiro MUST:
1. **Stop generation**: Do not output the resume
2. **Identify issues**: List specific validation failures
3. **Suggest corrections**: Provide specific guidance on how to fix issues
4. **Re-validate**: After corrections, run full validation again

## Validation Success Protocol
Only after ALL validation checks pass, Kiro may:
1. **Generate metadata**: Include proper generation metadata
2. **Output resume**: Save to resumes/ folder with proper naming
3. **Confirm compliance**: State that resume passes all steering file requirements

## Validation Reporting Format
For each generated resume, Kiro must provide a validation report:

```
RESUME VALIDATION REPORT
Generated: YYYY-MM-DD HH:MM
Target Role: {role-name}
File: resumes/{filename}

STEERING FILE COMPLIANCE:
✅ 00_mission.md - Mission compliance verified
✅ 01_repo_map.md - Repository structure compliance verified  
✅ 02_content_model.md - Content model compliance verified
✅ 03_writing_rules.md - Harvard writing standards verified
✅ 05_resume_assembly_rules.md - Assembly rules compliance verified
✅ 06_template.md - Template compliance verified

RESULT: ✅ PASS - Resume meets all steering file requirements
```

## Quality Metrics Tracking
For continuous improvement, track validation metrics:
- **Pass rate**: Percentage of resumes that pass validation on first attempt
- **Common failures**: Most frequent validation issues to address in steering files
- **Compliance trends**: Improvement in compliance over time

## Validation Automation
This validation process should be:
- **Automatic**: Runs on every resume generation without user intervention
- **Comprehensive**: Checks every requirement in every steering file
- **Blocking**: Prevents output of non-compliant resumes
- **Transparent**: Provides clear feedback on any failures
- **Consistent**: Same validation applied regardless of target role or industry
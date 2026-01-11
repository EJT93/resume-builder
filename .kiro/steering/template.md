---
inclusion: always
last_updated: "2026-01-11"
---

# Universal Resume Template - Predictable Structure

## Mandatory Resume Structure

Every generated resume MUST follow this exact structure and formatting:

### 1. Generation Metadata (Top of File)
```markdown
<!-- Generated: YYYY-MM-DD -->
<!-- Target Role: {role-name} -->
<!-- Template: .kiro/steering/template.md -->
<!-- Content Selected: {count} roles, {count} projects -->
<!-- Length: ~{word-count} words, {page-estimate} pages -->
```

### 2. Header Section
```markdown
# [Full Name]
([Phone]) | [Email] | [City, State/Country]
```

### 3. Education Section (Always Second)
```markdown
## Education

**[Institution Name]**, [City, State]  
[Degree Type], [Field of Study], [Graduation Date]
```

### 4. Professional Experience Section
```markdown
## Professional Experience

**[Job Title]** | [Company Name] | [Location] | [Start Date] - [End Date]
- [Action verb] + [context] + [quantified result in one line]
- [Action verb] + [context] + [quantified result in one line]
- [Action verb] + [context] + [quantified result in one line]
- [Action verb] + [context] + [quantified result in one line]

**[Previous Job Title]** | [Company Name] | [Location] | [Start Date] - [End Date]
- [Action verb] + [context] + [quantified result in one line]
- [Action verb] + [context] + [quantified result in one line]
- [Action verb] + [context] + [quantified result in one line]
- [Action verb] + [context] + [quantified result in one line]
```

### 5. Technical Skills Section
```markdown
## Technical Skills

**[Category 1]**: [Skill 1], [Skill 2], [Skill 3], [Skill 4]  
**[Category 2]**: [Skill 1], [Skill 2], [Skill 3], [Skill 4]  
**[Category 3]**: [Skill 1], [Skill 2], [Skill 3], [Skill 4]  
```

### 6. Certifications Section
```markdown
## Certifications

- **[Certification Name]** - [Issuing Organization] ([Date])
- **[Certification Name]** - [Issuing Organization] ([Date])
```

## Strict Formatting Rules

### Bullet Points (Non-Negotiable)
- **Exactly 4 bullets per role** (no more, no less)
- **One line maximum per bullet** (essential for Harvard compliance)
- **Start with strong action verb** (past tense for completed roles, present for current)
- **Include quantified metrics** (percentages, numbers, timeframes)
- **Follow CAR format**: Context + Action + Result

### Section Ordering (Fixed)
1. Header
2. Education (always second, regardless of experience level)
3. Professional Experience
4. Technical Skills
5. Certifications

### Content Selection Rules
- **Maximum 3 roles** for clean, focused presentation
- **Most recent 5-7 years** of experience only
- **Select most relevant roles** for target position
- **Prioritize quantified achievements** over responsibilities

### Skills Categorization
Group technical skills into exactly 3 categories:
- **Primary category**: Most relevant to target role (e.g., "Cloud Platforms", "Programming Languages")
- **Secondary category**: Supporting technologies (e.g., "Infrastructure & Automation", "Development Tools")
- **Tertiary category**: Specialized or domain-specific skills (e.g., "Monitoring", "Security")

## Dynamic Content Adaptation

### Role-Specific Emphasis
- **Technical roles**: Emphasize technical depth, system scale, performance metrics
- **Management roles**: Emphasize team leadership, business impact, strategic outcomes
- **Healthcare roles**: Emphasize patient outcomes, compliance, safety metrics
- **Finance roles**: Emphasize financial impact, risk management, regulatory compliance

### Industry-Appropriate Metrics
- **Technology**: Uptime percentages, performance improvements, cost savings, deployment frequency
- **Healthcare**: Patient satisfaction, safety improvements, compliance rates, efficiency gains
- **Finance**: Revenue impact, cost reductions, risk mitigation, accuracy improvements
- **Government**: Process improvements, cost savings, compliance adherence, citizen impact

### Action Verb Selection by Role Type
- **Technical**: Engineered, Developed, Implemented, Optimized, Automated, Deployed
- **Leadership**: Led, Managed, Directed, Coordinated, Spearheaded, Mentored
- **Process**: Streamlined, Enhanced, Improved, Reduced, Increased, Accelerated
- **Analysis**: Analyzed, Evaluated, Identified, Researched, Assessed, Investigated

## Quality Assurance Requirements

### Harvard Compliance Checklist
- [ ] Education section appears before Experience section
- [ ] All bullets are exactly one line
- [ ] Maximum 4 bullets per role
- [ ] No personal pronouns (I, me, my, we, us)
- [ ] Consistent parallel structure throughout
- [ ] Strong action verbs start each bullet
- [ ] All achievements include specific metrics

### Content Quality Standards
- [ ] All metrics are specific and verifiable
- [ ] No vague language ("significantly", "greatly", "many")
- [ ] Business impact clearly connected to technical work
- [ ] Industry-appropriate terminology used naturally
- [ ] Professional tone maintained throughout

### Formatting Consistency
- [ ] Consistent bullet point style (- or •)
- [ ] Consistent date formatting (Month YYYY)
- [ ] Consistent company/location formatting
- [ ] Consistent skill categorization format
- [ ] Clean, ATS-friendly markdown structure

## Quality Assurance Requirements

### Harvard Compliance Checklist
- [ ] Education section appears before Experience section
- [ ] All bullets are exactly one line
- [ ] Maximum 4 bullets per role
- [ ] No personal pronouns (I, me, my, we, us)
- [ ] Consistent parallel structure throughout
- [ ] Strong action verbs start each bullet
- [ ] All achievements include specific metrics

### Content Quality Standards
- [ ] All metrics are specific and verifiable
- [ ] No vague language ("significantly", "greatly", "many")
- [ ] Business impact clearly connected to technical work
- [ ] Industry-appropriate terminology used naturally
- [ ] Professional tone maintained throughout

### Formatting Consistency
- [ ] Consistent bullet point style (- or •)
- [ ] Consistent date formatting (Month YYYY)
- [ ] Consistent company/location formatting
- [ ] Consistent skill categorization format
- [ ] Clean, ATS-friendly markdown structure

### Validation Protocol
Before outputting any resume, Kiro MUST verify:
1. **Mission compliance**: All content sourced from profile/experience files, no fabrication
2. **Structure compliance**: Follows exact template structure and Harvard standards
3. **Content quality**: All bullets quantified, professional tone, no TODO markers
4. **File placement**: Resume saved to `resumes/{target-role}-{date}.md`

This template ensures every resume has the same professional structure and formatting while allowing dynamic content selection based on target role and industry requirements.
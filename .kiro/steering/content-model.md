---
inclusion: always
---

# Content Model and Structure

## Experience File Structure

### Roles File (`experience/roles.md`)

Contains all professional positions in a single file:
```markdown
---
type: "roles"
last_updated: "YYYY-MM-DD"
---

# Professional Experience

## Role 1: {Job Title} at {Company Name}
**Duration**: {Start Date} - {End Date}  
**Location**: {City, State/Country}  
**Tags**: ["industry", "role-type", "seniority-level"]

### Overview
Brief description of the role and its context within the organization.

### Key Responsibilities
- Bullet point describing primary responsibility
- Another key responsibility with specific scope
- Third responsibility showing impact area

### Notable Achievements
- Quantified achievement with metrics
- Process improvement or efficiency gain
- Leadership or mentorship accomplishment

---

## Role 2: {Job Title} at {Company Name}
[Same structure as above]
```

### Projects File (`experience/projects.md`)

Contains all projects with company/role context:
```markdown
---
type: "projects"
last_updated: "YYYY-MM-DD"
---

# Professional Projects

## Project 1: {Project Name}
**Company/Role**: {Company Name} - {Role Title}  
**Duration**: {X months} or {YYYY-MM to YYYY-MM}  
**Technologies**: ["tech1", "tech2", "tech3"]  
**Tags**: ["project-type", "industry", "scale"]

### Context
Brief description of the business problem or opportunity.

### Solution
High-level description of the approach and your specific contributions.

### Impact
- Quantified business impact (revenue, cost savings, efficiency)
- Technical impact (performance improvements, scalability)
- User impact (adoption, satisfaction, engagement)

---

## Project 2: {Project Name}
[Same structure as above]
```

## Profile File Structure

All profile files follow similar patterns with frontmatter and structured content sections.

### Profile File Requirements

#### Identity File (`profile/identity.md`)
```markdown
---
type: "identity"
last_updated: "YYYY-MM-DD"
---

# Personal Identity

## Contact Information
**Full Name**: [Legal name for professional use]
**Phone**: [Primary contact number]
**Email**: [Professional email address]
**Location**: [City, State/Country]

## Professional Headline
[One-line professional headline that captures value proposition]
```

#### Skills File (`profile/skills.md`)
```markdown
---
type: "skills"
last_updated: "YYYY-MM-DD"
---

# Technical and Professional Skills

## [Category 1 Name]
[Skill 1], [Skill 2], [Skill 3], [Skill 4]

## [Category 2 Name]
[Skill 1], [Skill 2], [Skill 3], [Skill 4]

## [Category 3 Name]
[Skill 1], [Skill 2], [Skill 3], [Skill 4]
```

#### Education File (`profile/education.md`)
```markdown
---
type: "education"
last_updated: "YYYY-MM-DD"
---

# Educational Background

## [Degree Level] - [Field of Study]
**Institution**: [University/College Name]
**Location**: [City, State]
**Graduation**: [Month Year]
**GPA**: [If 3.5 or higher]
**Honors**: [Dean's List, Magna Cum Laude, etc.]
**Relevant Coursework**: [3-4 most relevant courses for target roles]
```

#### Certifications File (`profile/certifications.md`)
```markdown
---
type: "certifications"
last_updated: "YYYY-MM-DD"
---

# Professional Certifications

## Active Certifications
- **[Certification Name]** - [Issuing Organization] ([Date Earned])
- **[Certification Name]** - [Issuing Organization] ([Date Earned])

## In Progress
- **[Certification Name]** - [Issuing Organization] (Expected [Date])
```

## Content Quality Standards

### Required Elements for All Content
- **Frontmatter**: Every file must include type and last_updated
- **Structured headings**: Consistent heading hierarchy
- **Quantified achievements**: Include specific metrics wherever possible
- **Professional tone**: Industry-appropriate language
- **Tag consistency**: Use standardized tags for filtering

### Prohibited Content
- **Fabricated information**: Never invent facts, dates, or metrics
- **Vague language**: Avoid "significantly", "greatly", "many"
- **Personal pronouns**: Avoid I, me, my, we, us in final resume bullets
- **Unverifiable claims**: Avoid superlatives without supporting data
- **Confidential information**: Respect employer confidentiality

### Content Validation Rules
- All dates must be accurate and verifiable
- Company names must match official legal names
- Job titles must reflect actual positions held
- Achievements must be supportable with evidence
- Missing information marked with TODO, never invented
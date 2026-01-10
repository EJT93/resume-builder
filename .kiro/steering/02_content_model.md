# Content Model and Structure

## Atom Types and Required Structure

### Role Atoms (`library/roles/`)

Required Markdown structure:
```markdown
---
company: "Company Name"
title: "Job Title"
start_date: "YYYY-MM"
end_date: "YYYY-MM" # or "present"
location: "City, State/Country"
tags: ["industry", "role-type", "seniority-level"]
---

# {Job Title} at {Company Name}

## Overview
Brief description of the role and its context within the organization.

## Key Responsibilities
- Bullet point describing primary responsibility
- Another key responsibility with specific scope
- Third responsibility showing impact area

## Notable Achievements
- Quantified achievement with metrics
- Process improvement or efficiency gain
- Leadership or mentorship accomplishment
```

### Project Atoms (`library/projects/`)

Required Markdown structure:
```markdown
---
name: "Project Name"
duration: "X months" # or "YYYY-MM to YYYY-MM"
role: "Your role in project"
technologies: ["tech1", "tech2", "tech3"]
tags: ["project-type", "industry", "scale"]
---

# {Project Name}

## Context
Brief description of the business problem or opportunity.

## Solution
High-level description of the approach and your specific contributions.

## Impact
- Quantified business impact (revenue, cost savings, efficiency)
- Technical impact (performance improvements, scalability)
- User impact (adoption, satisfaction, engagement)

## Technologies Used
List of key technologies, frameworks, and tools.
```

### Achievement Atoms (`library/achievements/`)

Required Markdown structure:
```markdown
---
type: "award" # or "recognition", "milestone", "certification"
date: "YYYY-MM"
organization: "Awarding Organization"
tags: ["category", "level"]
---

# {Achievement Name}

## Description
What the achievement represents and why it's significant.

## Context
Circumstances that led to this achievement.

## Impact
How this achievement benefited you, your team, or organization.
```

### Skill Atoms (`library/skills/`)

Required Markdown structure:
```markdown
---
category: "Technical" # or "Leadership", "Communication", etc.
proficiency: "Expert" # or "Advanced", "Intermediate", "Beginner"
years_experience: X
tags: ["skill-type", "domain"]
---

# {Skill Category}

## Skills List
- Specific skill (proficiency level, years experience)
- Another skill (proficiency level, years experience)
- Third skill (proficiency level, years experience)

## Context
Brief description of how these skills were developed and applied.
```

### Certification Atoms (`library/certifications/`)

Required Markdown structure:
```markdown
---
name: "Certification Name"
issuer: "Issuing Organization"
date_earned: "YYYY-MM"
expiry_date: "YYYY-MM" # if applicable
credential_id: "ID123456" # if applicable
tags: ["certification-type", "domain"]
---

# {Certification Name}

## Description
What this certification validates and its industry significance.

## Requirements
Brief overview of what was required to earn this certification.
```

### Education Atoms (`library/education/`)

Required Markdown structure:
```markdown
---
degree: "Degree Type"
field: "Field of Study"
institution: "Institution Name"
graduation_date: "YYYY-MM"
gpa: "X.XX" # optional
location: "City, State/Country"
tags: ["degree-level", "field-category"]
---

# {Degree} in {Field} - {Institution}

## Relevant Coursework
- Course 1 (if relevant to target roles)
- Course 2 (if relevant to target roles)
- Course 3 (if relevant to target roles)

## Notable Projects or Achievements
- Academic project or research
- Awards or honors
- Leadership roles
```

## Frontmatter Standards

### Required Fields
All atoms must include:
- Appropriate type-specific fields (see above)
- `tags` array for filtering and selection

### Optional Fields
- `priority` (1-5, where 5 is highest priority for inclusion)
- `confidential` (boolean, excludes from certain views)
- `draft` (boolean, excludes from all resume generation)

### Tag Categories
- **Industry**: "fintech", "healthcare", "e-commerce", "enterprise"
- **Role Type**: "individual-contributor", "team-lead", "manager", "executive"
- **Seniority**: "junior", "mid-level", "senior", "staff", "principal"
- **Domain**: "backend", "frontend", "devops", "data", "security", "product"
- **Scale**: "startup", "mid-size", "enterprise", "global"
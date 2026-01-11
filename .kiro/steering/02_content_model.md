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
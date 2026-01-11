---
inclusion: always
---
# Repository Structure and Navigation

## Folder Hierarchy

```
.kiro/steering/     # All system behavior definitions (this folder)
├── mission.md      # Core purpose, principles, and guardrails
├── structure.md    # Repository organization and navigation (this file)
├── content-model.md # Content structure and quality standards
├── writing-rules.md # Harvard resume standards and formatting
├── validation.md   # Quality assurance and compliance checks
└── template.md     # Complete resume formatting and assembly rules
profile/           # Personal identity and contact information
experience/        # Professional experience content
├── roles.md       # All professional positions and responsibilities
└── projects.md    # All projects and initiatives
resumes/           # Generated resume files (gitignored)
```

## File Types and Naming Conventions

### Profile Files (Always Included)
- `profile/identity.md` - Name, title, location, contact info
- `profile/links.md` - Professional links (LinkedIn, GitHub, portfolio)
- `profile/summary.md` - Professional summary paragraphs for different contexts
- `profile/certifications.md` - Professional certifications with dates
- `profile/education.md` - Academic background and degrees
- `profile/skills.md` - Technical and professional skills

### Experience Content Files (Selectively Included)
- **Roles**: `experience/roles.md` - All professional positions in chronological order
- **Projects**: `experience/projects.md` - All projects with company/role context specified

### Content Structure Requirements

#### Roles File Format (`experience/roles.md`)
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
```

#### Projects File Format (`experience/projects.md`)
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
```

### Steering Files
- `mission.md` - Core purpose, principles, and guardrails for the resume-as-code system
- `structure.md` - Repository organization, file relationships, and navigation guide
- `content-model.md` - Detailed content structure requirements and quality standards
- `writing-rules.md` - Harvard resume standards, formatting rules, and style guidelines
- `validation.md` - Comprehensive quality assurance and compliance validation process
- `template.md` - Complete resume formatting structure and assembly rules

## Adding New Content

### New Content
1. Add new roles to `experience/roles.md` following the content model structure
2. Add new projects to `experience/projects.md` with company/role context
3. Use consistent formatting and include relevant tags for filtering

### Steering File Updates
1. Modify `.kiro/steering/template.md` to adjust universal resume generation rules
2. Update `.kiro/steering/writing-rules.md` for Harvard formatting standards
3. Modify `.kiro/steering/content-model.md` for content structure requirements
4. Update `.kiro/steering/validation.md` for quality assurance processes
5. Add industry-specific guidance while maintaining universal applicability

## File Relationships

- **Steering files** work together to define complete system behavior:
  - `mission.md` establishes core principles and guardrails
  - `structure.md` defines organization and file relationships
  - `content-model.md` specifies detailed content structure requirements
  - `writing-rules.md` enforces Harvard resume standards and formatting
  - `validation.md` ensures quality assurance and compliance
  - `template.md` provides complete formatting and assembly framework
- **Profile files** are automatically included in all resumes
- **Experience files** contain multiple entries that can be selectively included
- **Content selection** is dynamic based on user prompts and target roles
- **Kiro applies** intelligent filtering and emphasis based on all steering file guidelines
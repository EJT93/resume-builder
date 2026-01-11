---
inclusion: always
---
# Repository Structure and Navigation

## Folder Hierarchy

```
.kiro/steering/     # All system behavior definitions (this folder)
profile/           # Personal identity and contact information
experience/        # Professional experience content
├── roles.md       # All professional positions and responsibilities
└── projects.md    # All projects and initiatives
resumes/           # Generated resume files (gitignored)
```

## File Types and Naming Conventions

### Profile Files
- `profile/identity.md` - Name, title, location, contact info
- `profile/links.md` - Professional links (LinkedIn, GitHub, portfolio)
- `profile/summary.md` - Professional summary paragraphs for different contexts
- `profile/certifications.md` - Professional certifications with dates
- `profile/education.md` - Academic background and degrees
- `profile/skills.md` - Technical and professional skills

### Experience Content Files
- **Roles**: `experience/roles.md` - All professional positions in chronological order
- **Projects**: `experience/projects.md` - All projects with company/role context specified

### Universal Template
- `06_template.md` - Universal resume template that works for any profession or industry

## Adding New Content

### New Content
1. Add new roles to `experience/roles.md` following the content model structure
2. Add new projects to `experience/projects.md` with company/role context
3. Use consistent formatting and include relevant tags for filtering

### New Template Updates
1. Modify `.kiro/steering/06_template.md` to adjust universal resume generation rules
2. Update content selection criteria or formatting preferences
3. Add industry-specific guidance while maintaining universal applicability

## File Relationships

- Universal template provides framework for all resume generation
- Experience files contain multiple entries that can be selectively included
- Profile files are automatically included in all resumes
- Content selection is dynamic based on user prompts and target roles
- Kiro applies intelligent filtering and emphasis based on template guidelines
# Repository Structure and Navigation

## Folder Hierarchy

```
.kiro/steering/     # All system behavior definitions (this folder)
profile/           # Personal identity and contact information
experience/        # Professional experience content
├── roles.md       # All professional positions and responsibilities
└── projects.md    # All projects and initiatives
views/             # Resume view definitions for different roles/industries
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

### View Definitions
- `views/{target-role}.view.md` - Defines how to assemble resume for specific role types
- Examples: `platform-engineer.view.md`, `product-manager.view.md`, `data-scientist.view.md`

## Adding New Content

### New Content
1. Add new roles to `experience/roles.md` following the content model structure
2. Add new projects to `experience/projects.md` with company/role context
3. Use consistent formatting and include relevant tags for filtering

### New View Definitions
1. Create `.view.md` file in views/ folder
2. Define target role, required atoms, ordering rules
3. Specify length constraints and emphasis areas
4. Reference existing atoms by filename

## File Relationships

- Views reference content from experience files by section or tags
- Experience files contain multiple entries that can be selectively included
- Profile files are automatically included in all resumes
- Tags and priorities within experience files enable filtering and selection logic
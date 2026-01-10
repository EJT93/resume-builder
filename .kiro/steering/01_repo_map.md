# Repository Structure and Navigation

## Folder Hierarchy

```
.kiro/steering/     # All system behavior definitions (this folder)
profile/           # Personal identity and contact information
library/           # Reusable content atoms organized by type
├── roles/         # Professional positions and responsibilities
├── projects/      # Specific projects and initiatives
├── achievements/  # Awards, recognitions, and notable accomplishments
├── skills/        # Technical and soft skills with proficiency levels
├── certifications/ # Professional certifications and licenses
└── education/     # Academic background and training
views/             # Resume view definitions for different roles/industries
output/            # Generated resume files (gitignored)
```

## File Types and Naming Conventions

### Profile Files
- `profile/identity.md` - Name, title, location, contact info
- `profile/links.md` - Professional links (LinkedIn, GitHub, portfolio)
- `profile/summary.md` - Professional summary paragraphs for different contexts

### Library Content Atoms
- **Roles**: `library/roles/{job-title-company}.md` (e.g., `senior-engineer-acme.md`)
- **Projects**: `library/projects/{project-name}.md` (e.g., `payment-system-redesign.md`)
- **Achievements**: `library/achievements/{achievement-name}.md` (e.g., `aws-certification.md`)
- **Skills**: `library/skills/{skill-category}.md` (e.g., `cloud-platforms.md`)
- **Certifications**: `library/certifications/{cert-name}.md` (e.g., `pmp-certification.md`)
- **Education**: `library/education/{degree-institution}.md` (e.g., `bs-computer-science-mit.md`)

### View Definitions
- `views/{target-role}.view.md` - Defines how to assemble resume for specific role types
- Examples: `platform-engineer.view.md`, `product-manager.view.md`, `data-scientist.view.md`

## Adding New Content

### New Content Atoms
1. Create file in appropriate library subfolder
2. Use kebab-case naming convention
3. Follow content model structure from `02_content_model.md`
4. Add relevant tags in frontmatter for filtering

### New View Definitions
1. Create `.view.md` file in views/ folder
2. Define target role, required atoms, ordering rules
3. Specify length constraints and emphasis areas
4. Reference existing atoms by filename

## File Relationships

- Views reference atoms by filename (without extension)
- Atoms are self-contained and don't reference each other
- Profile files are automatically included in all resumes
- Tags in frontmatter enable filtering and selection logic
# Resume-as-Code Repository

A personal knowledge base of reusable resume content managed through Kiro IDE steering files.

## What is Resume-as-Code?

Resume-as-code treats your professional history like source code:
- **Atomic content**: Each role, project, achievement exists as a separate Markdown file
- **Version controlled**: All changes tracked in git
- **Reusable**: Content atoms mixed and matched for different opportunities  
- **Consistent**: Standardized formats ensure quality and ATS compatibility
- **Maintainable**: Updates to atoms automatically improve all resumes

## Repository Structure

```
.kiro/steering/     # System behavior definitions
profile/           # Personal identity and contact information
library/           # Reusable content atoms
├── roles/         # Professional positions
├── projects/      # Specific projects and initiatives  
├── achievements/  # Awards and recognitions
├── skills/        # Technical and soft skills
├── certifications/ # Professional certifications
└── education/     # Academic background
views/             # Resume assembly definitions for different roles
output/            # Generated resume files (gitignored)
```

## How It Works

1. **Store content as atoms**: Each experience, skill, or achievement is a separate Markdown file
2. **Define assembly rules**: View files specify how to select and arrange content for different roles
3. **Generate tailored resumes**: Kiro IDE uses steering files to assemble targeted resumes
4. **Maintain accuracy**: All facts stored once, TODO markers for missing information

## Getting Started

### 1. Update Your Profile
Edit files in `profile/` folder:
- `identity.md` - Contact information and basic details
- `links.md` - Professional URLs and social profiles  
- `summary.md` - Professional summary variants for different contexts

### 2. Add Your Experience
Create files in `library/` subfolders following the content model:
- Use the question bank in `.kiro/steering/04_question_bank.md` to gather details
- Follow writing rules in `.kiro/steering/03_writing_rules.md`
- Mark missing information with TODO instead of inventing facts

### 3. Create View Definitions
Define how resumes should be assembled in `views/` folder:
- Specify target role requirements and preferences
- Set content selection and ordering rules
- Configure length and emphasis guidelines

### 4. Generate Resumes
Use Kiro IDE with natural language prompts:
- "Generate a platform engineer resume"
- "Create a resume targeting senior backend roles"
- "Assemble a 1-page resume for startup positions"

## Key Principles

- **Truth in one place**: Each fact exists in exactly one file
- **No fabrication**: Missing information marked with TODO, never invented
- **Universal applicability**: Works for any profession, not just engineering
- **Markdown-only**: No scripts, templates, or complex tooling
- **Steering-driven**: All behavior defined in `.kiro/steering/` files

## Steering Files Reference

- `00_mission.md` - Purpose and principles
- `01_repo_map.md` - Structure and navigation
- `02_content_model.md` - Atom types and formats
- `03_writing_rules.md` - Quality and style standards
- `04_question_bank.md` - Content development questions
- `05_resume_assembly_rules.md` - Selection and ordering logic

## Example Usage

```
# In Kiro IDE chat
"I need a resume for a DevOps engineer position at a fintech startup. 
Emphasize automation and scalability experience, keep it to 1.5 pages."

# Kiro will:
1. Reference steering files for assembly rules
2. Select relevant atoms based on tags and priorities
3. Order content according to view definition
4. Generate tailored resume in output/ folder
```

## Contributing to Your Own Repository

1. **Add new experiences**: Create atoms in appropriate library folders
2. **Update existing content**: Edit atoms to add metrics or refine descriptions
3. **Create new views**: Define assembly rules for different target roles
4. **Refine steering**: Update rules based on what works best for your career

## Privacy and Security

- Generated resumes in `output/` folder should be gitignored
- Consider using private repository for personal information
- Review all content before sharing or publishing
- Use TODO markers instead of placeholder personal data
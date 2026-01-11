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
├── identity.md    # Contact info and professional headline
├── links.md       # Professional URLs and profiles
├── summary.md     # Professional summary variants
├── certifications.md # Professional certifications
├── education.md   # Academic background
└── skills.md      # Technical and professional skills
experience/        # Professional experience content
├── roles.md       # All professional positions
└── projects.md    # All projects and initiatives
views/             # Resume assembly definitions for different roles
resumes/           # Generated resume files (gitignored)
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
- `certifications.md` - Professional certifications with dates

### 2. Add Your Experience
Update files in `experience/` folder:
- `roles.md` - Add all your professional positions with achievements
- `projects.md` - Add all your projects with company/role context
- Follow Harvard resume standards and mark missing info with TODO

### 3. Create View Definitions
Define how resumes should be assembled in `views/` folder:
- Specify target role requirements and preferences
- Set content selection and ordering rules
- Configure length and emphasis guidelines

### 4. Generate Resumes
Use Kiro IDE with natural language prompts:
- "Generate a platform engineer resume following Harvard standards"
- "Create a resume targeting senior backend roles at fintech companies"
- "Assemble a 1-page resume for startup engineering positions"

## Key Principles

- **Truth in one place**: Each fact exists in exactly one file
- **No fabrication**: Missing information marked with TODO, never invented
- **Universal applicability**: Works for any profession, not just engineering
- **Markdown-only**: No scripts, templates, or complex tooling
- **Steering-driven**: All behavior defined in `.kiro/steering/` files

## Steering Files Reference

- `00_mission.md` - Purpose and principles
- `01_repo_map.md` - Structure and navigation
- `02_content_model.md` - Atom types and Harvard-compliant formats
- `03_writing_rules.md` - Harvard resume standards and quality guidelines
- `04_question_bank.md` - Kiro's direct resume generation approach
- `05_resume_assembly_rules.md` - Selection and ordering logic

## Example Usage

```
# In Kiro IDE chat
"I need a resume for a DevOps engineer position at a fintech startup. 
Use Harvard resume format, emphasize automation and scalability experience, keep it to 1 page."

# Kiro will:
1. Reference steering files for Harvard formatting and assembly rules
2. Select relevant atoms based on tags, recency, and impact scores
3. Apply fintech industry terminology and compliance focus
4. Generate Harvard-standard resume in resumes/ folder with proper formatting
```

## Contributing to Your Own Repository

1. **Add new experiences**: Update `experience/roles.md` and `experience/projects.md`
2. **Update existing content**: Edit entries to add metrics or refine descriptions
3. **Create new views**: Define assembly rules for different target roles
4. **Refine steering**: Update rules based on what works best for your career

## Privacy and Security

- Generated resumes in `resumes/` folder should be gitignored
- Consider using private repository for personal information
- Review all content before sharing or publishing
- Use TODO markers instead of placeholder personal data
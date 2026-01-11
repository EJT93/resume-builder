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
resumes/           # Generated resume files (gitignored)
```

## How It Works

1. **Store content as atoms**: Each experience, skill, or achievement is stored in structured Markdown files
2. **Follow Harvard standards**: All content follows Harvard resume formatting and quality requirements
3. **Universal template**: Single template structure adapts to any profession or industry
4. **Automatic validation**: Every generated resume passes comprehensive quality assurance checks
5. **Create targeted resumes**: Kiro IDE assembles resumes using natural language prompts
6. **Maintain accuracy**: All facts stored once, TODO markers for missing information

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

### 3. Generate Resumes
Use Kiro IDE with natural language prompts for any profession:
- "Generate a platform engineer resume following Harvard standards"
- "Create a healthcare administrator resume emphasizing patient outcomes"
- "Assemble a marketing manager resume for fintech companies"
- "Build a 1-page resume for entry-level data analyst positions"

## Key Principles

- **Truth in one place**: Each fact exists in exactly one file
- **No fabrication**: Missing information marked with TODO, never invented
- **Harvard compliance**: All resumes follow Harvard Business School formatting standards
- **Universal applicability**: Works for any profession, not just engineering
- **Validation-first**: Every resume passes comprehensive quality assurance before output
- **Markdown-only**: No scripts, templates, or complex tooling
- **Steering-driven**: All behavior defined in `.kiro/steering/` files

## Steering Files Reference

- `mission.md` - Core purpose, principles, and guardrails
- `structure.md` - Repository organization and file relationships
- `content-model.md` - Content structure requirements and quality standards
- `writing-rules.md` - Harvard resume standards and formatting rules
- `validation.md` - Comprehensive quality assurance and compliance checks
- `template.md` - Universal resume formatting and assembly rules

## Example Usage

```
# In Kiro IDE chat
"I need a resume for a DevOps engineer position at a fintech startup. 
Use Harvard resume format, emphasize automation and scalability experience, keep it to 1 page."

# Kiro will:
1. Apply universal template with Harvard formatting standards from steering files
2. Select relevant content from roles.md and projects.md based on DevOps keywords
3. Adapt technical terminology and emphasis for fintech industry requirements
4. Run comprehensive validation against all steering file requirements
5. Generate compliant resume in resumes/ folder with proper naming convention
6. Provide validation report confirming Harvard standards compliance
```

## Contributing to Your Own Repository

1. **Add new experiences**: Update `experience/roles.md` and `experience/projects.md`
2. **Update existing content**: Edit entries to add metrics or refine descriptions
3. **Refine steering**: Update rules and template based on what works best across different professions

## Privacy and Security

- Generated resumes in `resumes/` folder should be gitignored
- Consider using private repository for personal information
- Review all content before sharing or publishing
- Use TODO markers instead of placeholder personal data
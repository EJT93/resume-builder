# Resume Assembly Rules and Logic

## Content Selection Process

### Atom Selection Criteria
1. **Relevance Scoring**: Match atom tags to target role requirements
2. **Recency Weighting**: Prioritize more recent experiences (last 5-10 years)
3. **Impact Prioritization**: Select atoms with strongest quantified achievements
4. **Diversity Balance**: Include variety of experience types and contexts
5. **Tag Filtering**: Use view-specific tag requirements to include/exclude content

### Selection Algorithm
```
For each atom in library:
  Calculate relevance_score = tag_match_count * tag_weight
  Calculate recency_score = years_ago_factor * recency_weight  
  Calculate impact_score = metric_strength * impact_weight
  Calculate priority_score = frontmatter_priority * priority_weight
  
  Total_score = relevance_score + recency_score + impact_score + priority_score
  
Sort atoms by total_score descending
Select top N atoms based on resume length constraints
```

### Mandatory Inclusions
- All profile atoms (identity, links, summary) are always included
- Current role (if end_date = "present") is always included
- Any atom with `priority: 5` in frontmatter is always included
- Education atoms for roles requiring specific degrees

### Automatic Exclusions
- Atoms with `draft: true` in frontmatter
- Atoms with `confidential: true` when generating public resumes
- Roles older than 15 years (unless specifically high-impact)
- Duplicate or overlapping project descriptions

## Ordering and Prioritization Rules

### Section Order (Standard)
1. Contact Information (from profile/identity.md)
2. Professional Summary (from profile/summary.md, tailored to view)
3. Professional Experience (roles, ordered by end_date descending)
4. Key Projects (if not integrated into roles, ordered by impact/recency)
5. Technical Skills (from skills atoms, grouped by category)
6. Education (ordered by graduation_date descending)
7. Certifications (ordered by date_earned descending)
8. Notable Achievements (if not integrated elsewhere)

### Within-Section Ordering
- **Roles**: Reverse chronological (most recent first)
- **Projects**: By impact score, then recency
- **Skills**: By proficiency level, then relevance to target role
- **Achievements**: By significance, then recency
- **Education**: Reverse chronological

### Content Prioritization Within Atoms
- Lead with highest-impact bullets (quantified achievements)
- Follow with core responsibilities that match target role
- End with supporting context or additional relevant details
- Limit to 3-5 bullets per role, 2-3 bullets per project

## Length and Emphasis Constraints

### Resume Length Guidelines
- **Junior roles (0-3 years)**: Target 1 page, maximum 1.5 pages
- **Mid-level roles (3-8 years)**: Target 1.5 pages, maximum 2 pages  
- **Senior roles (8+ years)**: Target 2 pages, maximum 2.5 pages
- **Executive roles**: 2-3 pages acceptable

### Content Allocation by Experience Level
**Junior (1 page)**:
- 20% Contact + Summary
- 50% Professional Experience (2-3 roles max)
- 15% Education (more detailed)
- 10% Skills
- 5% Projects/Achievements

**Senior (2 pages)**:
- 15% Contact + Summary  
- 60% Professional Experience (4-5 roles max)
- 15% Key Projects
- 7% Skills
- 3% Education (brief)

### Emphasis Rules
- **High emphasis**: Current role gets 40% more detail than others
- **Medium emphasis**: Last 2-3 roles get full treatment
- **Low emphasis**: Older roles get condensed to 1-2 bullets
- **Skill emphasis**: Match target role requirements with 80%+ coverage

## Rewriting and Adaptation Rules

### Allowed Modifications
- **Bullet reordering**: Prioritize most relevant achievements first
- **Language adaptation**: Adjust technical depth for target audience
- **Keyword optimization**: Include target role terminology naturally
- **Emphasis shifting**: Highlight most relevant aspects of each experience
- **Metric contextualization**: Add industry context to numbers when helpful

### Prohibited Modifications
- **Fact alteration**: Never change dates, companies, titles, or metrics
- **Experience invention**: Never add roles, projects, or achievements that didn't happen
- **Metric fabrication**: Never invent or exaggerate quantified results
- **Responsibility inflation**: Never claim authority or scope beyond actual experience

### Rewriting Guidelines
- Maintain truthfulness while optimizing presentation
- Use stronger action verbs when accurate
- Add context that makes achievements more impressive
- Remove irrelevant details to focus on target role alignment
- Ensure consistency in tone and formatting across all sections

## Output Generation Rules

### File Naming Convention
- `resumes/{target-role}-{date}.md` for dated versions
- `resumes/{target-role}-latest.md` for current version
- `resumes/{target-role}-{company}.md` for company-specific versions

### Metadata Inclusion
Include generation metadata at top of output file:
```markdown
<!-- Generated: YYYY-MM-DD HH:MM -->
<!-- Target Role: {role-name} -->
<!-- View Definition: {view-file} -->
<!-- Atoms Used: {count} total -->
<!-- Length: {word-count} words, {page-estimate} pages -->
```

### Quality Assurance Checks
Before finalizing output:
- Verify all dates are consistent and logical
- Confirm no TODO markers remain in final version
- Check that resume length meets target constraints
- Validate that all required sections are present
- Ensure ATS-friendly formatting throughout

### Version Control Integration
- Generate new resume file for each assembly run
- Maintain history of generated resumes in resumes/ folder
- Include git commit hash in metadata for traceability
- Tag significant resume versions for easy reference

## View-Specific Overrides

### Custom Selection Rules
Views can override default selection with:
- `required_tags`: Force inclusion of atoms with specific tags
- `excluded_tags`: Force exclusion of atoms with specific tags  
- `max_roles`: Limit number of professional roles included
- `emphasis_areas`: Specify which aspects to highlight

### Custom Ordering Rules
Views can specify:
- Alternative section ordering for industry norms
- Custom within-section prioritization logic
- Specific skill groupings or presentations
- Project integration vs. separate section preferences

### Length Customization
Views can override:
- Target page length for specific role types
- Section allocation percentages
- Bullet point limits per role/project
- Detail level for different experience periods
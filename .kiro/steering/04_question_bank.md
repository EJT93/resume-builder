# Kiro Resume Generation Guidelines

## Direct Resume Generation Approach

Kiro generates resumes directly based on role requirements without requiring extensive user interviews. The system uses intelligent content selection and Harvard resume standards to create professional, targeted resumes.

## Role-Based Content Selection

### Automatic Content Prioritization
When generating a resume for a specific role, Kiro automatically:
- **Analyzes target role requirements** from job descriptions or role type
- **Selects most relevant atoms** based on tag matching and relevance scoring
- **Prioritizes recent experience** (last 5-10 years) over older roles
- **Emphasizes quantified achievements** that demonstrate impact
- **Adapts language and terminology** to match industry standards

### Content Selection Algorithm
```
For target role:
1. Identify required skills and experience from role type
2. Score all atoms based on tag relevance and recency
3. Select top-scoring atoms within length constraints
4. Order content by impact and relevance
5. Apply Harvard formatting standards
6. Generate final resume with metadata
```

## Role-Specific Generation Rules

### Engineering Roles (Platform, Backend, Frontend, DevOps)
- **Emphasize**: Technical skills, system scale, performance metrics
- **Prioritize**: Recent technical projects, architecture decisions, automation
- **Include**: Relevant certifications, open source contributions
- **Language**: Technical depth appropriate for engineering audience

### Management Roles (Engineering Manager, Director, VP)
- **Emphasize**: Team leadership, business impact, strategic initiatives
- **Prioritize**: People management experience, budget responsibility, growth metrics
- **Include**: Team size, retention rates, process improvements
- **Language**: Balance of technical credibility and business acumen

### Product Roles (Product Manager, Product Owner, Strategy)
- **Emphasize**: User impact, business metrics, cross-functional collaboration
- **Prioritize**: Product launches, user growth, revenue impact
- **Include**: Market research, user research, A/B testing experience
- **Language**: Business-focused with technical understanding

### Sales/Business Development Roles
- **Emphasize**: Revenue generation, quota achievement, relationship building
- **Prioritize**: Sales metrics, deal sizes, territory growth
- **Include**: CRM experience, pipeline management, customer success
- **Language**: Results-oriented with clear financial impact

## Industry-Specific Adaptations

### Technology/Software Industry
- **Technical depth**: Include specific technologies, frameworks, architectures
- **Scale metrics**: User counts, transaction volumes, system performance
- **Innovation focus**: New technologies adopted, technical leadership
- **Collaboration**: Cross-functional work, technical mentoring

### Financial Services/Fintech
- **Compliance emphasis**: Regulatory knowledge, security standards
- **Risk management**: Risk assessment, mitigation strategies
- **Scale and reliability**: Transaction volumes, uptime requirements
- **Business impact**: Revenue generation, cost reduction, efficiency

### Healthcare/Biotech
- **Regulatory compliance**: HIPAA, FDA, clinical trial standards
- **Patient impact**: Patient outcomes, safety improvements
- **Research focus**: Clinical research, data analysis, publications
- **Collaboration**: Cross-disciplinary teams, medical professionals

### Consulting/Professional Services
- **Client impact**: Client satisfaction, project success rates
- **Business development**: New client acquisition, relationship management
- **Expertise demonstration**: Industry knowledge, thought leadership
- **Project management**: Multiple concurrent projects, stakeholder management

## Experience Level Adaptations

### Junior Level (0-3 years)
- **Education emphasis**: Relevant coursework, academic projects, GPA if 3.5+
- **Internship details**: Specific contributions and learning outcomes
- **Skill development**: Training completed, certifications earned
- **Project focus**: Individual contributions and technical growth

### Mid-Level (3-8 years)
- **Technical expertise**: Deep skills in specific areas, problem-solving
- **Project leadership**: Leading initiatives, mentoring junior team members
- **Business impact**: Quantified contributions to team and company goals
- **Professional growth**: Career progression, expanding responsibilities

### Senior Level (8+ years)
- **Strategic impact**: Influence on company direction, architectural decisions
- **Leadership experience**: Team building, cross-functional collaboration
- **Industry expertise**: Thought leadership, speaking, publications
- **Mentorship**: Developing others, knowledge sharing, culture building

## Automatic Content Enhancement

### Kiro's Content Optimization
When generating resumes, Kiro automatically:
- **Strengthens action verbs**: Replaces weak verbs with Harvard-approved alternatives
- **Adds business context**: Connects technical work to business outcomes
- **Quantifies impact**: Emphasizes metrics and measurable results
- **Optimizes keywords**: Includes industry-standard terminology
- **Ensures consistency**: Maintains parallel structure and formatting

### Quality Assurance Checks
Before finalizing resumes, Kiro verifies:
- **Harvard format compliance**: Proper structure, length, and formatting
- **ATS compatibility**: Clean formatting, appropriate keywords
- **Content accuracy**: No TODO markers in final output
- **Professional tone**: Appropriate language for target role and industry
- **Completeness**: All required sections present and properly formatted
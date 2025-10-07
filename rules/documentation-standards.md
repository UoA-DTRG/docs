# Documentation Standards

This document outlines the standards and best practices for writing documentation in the DTRG team.

## General Principles

1. **Clarity**: Write for your audience. Use clear, simple language.
2. **Consistency**: Follow established patterns and templates.
3. **Completeness**: Include all necessary information for understanding.
4. **Maintenance**: Keep documentation up-to-date with code changes.

## Document Structure

### Required Sections

Every documentation file should include:

1. **Title**: Clear, descriptive title (H1)
2. **Metadata**: Status, last updated, etc. (when applicable)
3. **Overview**: Brief description of the document's purpose
4. **Content**: Main body organized with clear headings
5. **Related Links**: References to related documentation

### Optional Sections

Include when relevant:
- Prerequisites
- Examples
- Troubleshooting
- FAQ
- Next steps

## Markdown Style

### File Names

- Use lowercase with hyphens: `my-document.md`
- Be descriptive but concise
- Match the document title when possible

### Headings

```markdown
# H1 - Document Title (only one per document)
## H2 - Major sections
### H3 - Subsections
#### H4 - Minor subsections
```

- Use ATX-style headers (`#` prefix)
- Include a space after the `#`
- Don't skip heading levels
- Use sentence case (capitalize first word only)

### Lists

**Unordered lists** for non-sequential items:
```markdown
- Item one
- Item two
  - Nested item
```

**Ordered lists** for sequential steps:
```markdown
1. First step
2. Second step
3. Third step
```

**Task lists** for checklists:
```markdown
- [x] Completed item
- [ ] Incomplete item
```

### Code

**Inline code** for short snippets:
```markdown
Use `code` for file names, commands, and inline code.
```

**Code blocks** for longer examples:
````markdown
```python
def example():
    return "Always specify the language"
```
````

### Links

**Internal links** (preferred for docs within repo):
```markdown
[Guide Name](../guides/guide-name.md)
```

**External links**:
```markdown
[External Resource](https://example.com)
```

**Section links**:
```markdown
[Jump to section](#section-heading)
```

### Emphasis

- **Bold** for important terms or emphasis
- *Italic* for subtle emphasis or terms
- `Code formatting` for code, commands, files

### Images

```markdown
![Descriptive alt text](path/to/image.png)
```

- Always include descriptive alt text
- Store images in an `images/` directory
- Use relative paths

## Content Guidelines

### Writing Style

- Use active voice
- Be concise but complete
- Use present tense
- Avoid jargon (or explain it)
- Write in second person ("you") for guides

### Code Examples

- Test all code examples before documenting
- Include necessary imports and context
- Show expected output when relevant
- Comment complex code
- Use realistic examples

### Step-by-Step Instructions

1. Number sequential steps
2. Start each step with a verb
3. Include expected outcomes
4. Provide troubleshooting for common issues
5. Keep steps focused and atomic

### Screenshots

- Include screenshots for UI elements
- Annotate screenshots when helpful
- Keep screenshots up-to-date
- Use consistent image sizes

## Templates

Use the appropriate template from `/templates`:

- **Project**: [project-template/README.md](../templates/project-template/README.md)
- **Guide**: [guide-template.md](../templates/guide-template.md)
- **Feature**: [feature-template.md](../templates/feature-template.md)
- **Meeting Notes**: [meeting-notes-template.md](../templates/meeting-notes-template.md)

## Documentation Types

### API Documentation

Include:
- Endpoint URLs
- HTTP methods
- Parameters (required/optional)
- Request/response examples
- Status codes
- Authentication requirements

### Architecture Documentation

Include:
- System overview
- Component diagrams
- Data flow
- Technology stack
- Design decisions and rationale

### Setup Guides

Include:
- Prerequisites
- Installation steps
- Configuration
- Verification
- Troubleshooting

## Review Checklist

Before submitting documentation:

- [ ] Spelling and grammar checked
- [ ] All links tested and working
- [ ] Code examples tested
- [ ] Appropriate template used
- [ ] Consistent formatting
- [ ] Clear and concise writing
- [ ] Index files updated
- [ ] Metadata complete (dates, status, etc.)

## Maintenance

### Keeping Docs Current

- Update documentation when changing code
- Review documentation regularly (quarterly)
- Mark outdated docs clearly
- Archive or remove obsolete documentation

### Version Information

Include version information when relevant:
- Feature version numbers
- API versions
- Compatible software versions
- Last update date

## Tools and Helpers

### Recommended Tools

- **Markdown editors**: VS Code with markdown extensions
- **Linters**: markdownlint
- **Spell checkers**: Built-in editor spell checkers
- **Link checkers**: markdown-link-check

### Useful Resources

- [Markdown Cheatsheet](../templates/markdown-cheatsheet.md)
- [Contributing Guide](../CONTRIBUTING.md)
- [Style Guide](markdown-style-guide.md)

## Examples

### Good Documentation Example

```markdown
# User Authentication Setup

**Last Updated:** 2024-01-15

## Overview

This guide explains how to set up user authentication using JWT tokens.

## Prerequisites

- Node.js 14+
- PostgreSQL database
- Basic understanding of JWT

## Step 1: Install Dependencies

Install the required packages:

\`\`\`bash
npm install jsonwebtoken bcrypt
\`\`\`

Expected output:
\`\`\`
added 2 packages
\`\`\`

[Continue with more steps...]
```

## Questions?

If you have questions about documentation standards:
- Check the [Contributing Guide](../CONTRIBUTING.md)
- Ask in the team channel
- Open an issue for clarification

---

*These standards are living documents. Suggest improvements via PR!*

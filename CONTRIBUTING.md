# Contributing to DTRG Documentation

Thank you for contributing to the DTRG research team documentation! This guide will help you add and update documentation effectively.

## 📝 Documentation Philosophy

Our documentation aims to be:
- **Clear and Concise**: Easy to understand and navigate
- **Consistent**: Following the same structure and style
- **Up-to-date**: Reflecting current practices and systems
- **Accessible**: Useful for team members at all levels

## 🚀 Quick Start

1. **Fork/Clone** this repository
2. **Create a branch** for your documentation updates
3. **Make your changes** following the guidelines below
4. **Submit a pull request** with a clear description

## 📂 Documentation Structure

Our documentation is organized into four main sections:

- **`/projects`** - Project-specific documentation
- **`/guides`** - Step-by-step tutorials and how-to guides
- **`/features`** - Feature specifications and implementation details
- **`/rules`** - Team policies, standards, and guidelines

### Adding New Documentation

1. **Choose the right section** for your documentation
2. **Use the appropriate template** from `/templates`
3. **Follow naming conventions** (kebab-case, e.g., `my-new-guide.md`)
4. **Update the index file** (README.md) in that section

## ✍️ Writing Guidelines

### Markdown Best Practices

- Use clear, descriptive headings
- Include code examples where relevant
- Add links to related documentation
- Use lists and tables for better readability
- Include diagrams or screenshots when helpful

### Code Examples

Use fenced code blocks with language specification:

```python
def example():
    return "Use proper syntax highlighting"
```

### Formatting

- **Bold** for emphasis on important terms
- *Italics* for subtle emphasis
- `Code formatting` for commands, file names, and code elements
- Links: `[Link text](url)`

## 🎯 Documentation Types

### Project Documentation
When documenting a project:
1. Create a folder in `/projects/project-name/`
2. Use the project template from `/templates/project-template/`
3. Include: README, architecture, setup, and API docs (as needed)
4. Update `/projects/README.md` with a link to your project

### Guides
When writing a guide:
1. Create a file in `/guides/`
2. Use the guide template from `/templates/guide-template.md`
3. Structure it step-by-step
4. Include prerequisites and verification steps
5. Update `/guides/README.md` with a link to your guide

### Feature Documentation
When documenting a feature:
1. Create a file in `/features/` (or `/features/project-name/`)
2. Use the feature template from `/templates/feature-template.md`
3. Include requirements, architecture, and implementation details
4. Update `/features/README.md` with your feature

### Rules and Guidelines
When adding team guidelines:
1. Create a file in `/rules/`
2. Be clear and specific about the standard or policy
3. Include examples and rationale where helpful
4. Get team consensus before adding new rules
5. Update `/rules/README.md` with a link

## 🔍 Review Process

1. **Self-review**: Check your documentation for clarity and accuracy
2. **Spell-check**: Use a spell checker to catch typos
3. **Link verification**: Ensure all links work correctly
4. **Template compliance**: Verify you've followed the appropriate template

### Pull Request Guidelines

When submitting a PR:
- Use a clear, descriptive title
- Explain what documentation you've added/updated
- Reference any related issues
- Request review from relevant team members

## 📋 Documentation Checklist

Before submitting documentation, ensure:

- [ ] Content is clear and well-organized
- [ ] Appropriate template is used
- [ ] Code examples are tested and accurate
- [ ] All links work correctly
- [ ] Index files are updated
- [ ] Spelling and grammar are correct
- [ ] Follows markdown style guide
- [ ] Related documentation is cross-referenced

## 🔄 Updating Existing Documentation

When updating existing docs:
1. Keep the existing structure unless there's a good reason to change it
2. Update the "Last Updated" date
3. Document breaking changes clearly
4. Update related documentation if needed

## ❓ Questions or Suggestions

- Open an issue for questions about documentation
- Propose major structural changes in an issue first
- Join team discussions about documentation improvements

## 📚 Resources

- [Markdown Cheatsheet](templates/markdown-cheatsheet.md)
- [Documentation Templates](templates/)
- [Team Guidelines](rules/)

---

*Thank you for helping improve DTRG documentation!*

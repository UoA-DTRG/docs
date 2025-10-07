# Documentation Map

Visual guide to the DTRG documentation structure and how to navigate it.

## 📂 Repository Structure

```
docs/
├── README.md                          # Main entry point and navigation
├── CONTRIBUTING.md                    # How to contribute to documentation
├── .gitignore                        # Git ignore rules
│
├── 📁 projects/                      # Project-specific documentation
│   ├── README.md                     # Projects index
│   └── [project-name]/               # Individual project folders
│       ├── README.md                 # Project overview
│       ├── architecture.md           # System design
│       ├── setup.md                  # Installation guide
│       └── api.md                    # API documentation
│
├── 📁 guides/                        # Step-by-step guides & tutorials
│   ├── README.md                     # Guides index
│   ├── onboarding.md                 # New member onboarding
│   ├── git-workflow.md               # Git workflow guide
│   └── [other-guides].md             # Additional guides
│
├── 📁 features/                      # Feature implementation docs
│   ├── README.md                     # Features index
│   └── [feature-name].md             # Feature documentation
│
├── 📁 rules/                         # Team policies & standards
│   ├── README.md                     # Rules index
│   ├── documentation-standards.md    # Documentation guidelines
│   └── [other-standards].md          # Additional standards
│
└── 📁 templates/                     # Reusable templates
    ├── README.md                     # Templates index
    ├── guide-template.md             # Guide template
    ├── feature-template.md           # Feature template
    ├── meeting-notes-template.md     # Meeting notes template
    ├── markdown-cheatsheet.md        # Markdown reference
    └── project-template/             # Project template folder
        └── README.md                 # Project template
```

## 🗺️ Documentation Journey

### For New Team Members

```
Start Here
    ↓
README.md → Get overview of documentation
    ↓
guides/onboarding.md → Complete onboarding
    ↓
guides/git-workflow.md → Learn our Git workflow
    ↓
projects/README.md → Browse active projects
    ↓
Start Contributing!
```

### For Documentation Writers

```
Need to Document Something?
    ↓
CONTRIBUTING.md → Understand contribution process
    ↓
Choose Documentation Type:
    ├── Project? → templates/project-template/
    ├── Guide? → templates/guide-template.md
    ├── Feature? → templates/feature-template.md
    └── Meeting? → templates/meeting-notes-template.md
    ↓
Write Documentation
    ↓
Update Index Files (section README.md)
    ↓
Submit Pull Request
```

### For Finding Information

```
Need Information?
    ↓
README.md → Browse by category
    ↓
├── Projects? → projects/README.md
├── How-to? → guides/README.md
├── Features? → features/README.md
└── Standards? → rules/README.md
    ↓
Navigate to specific document
```

## 📋 Document Types & Their Purpose

| Type | Location | Purpose | Template |
|------|----------|---------|----------|
| **Project Documentation** | `/projects` | Complete project information | [project-template](templates/project-template/) |
| **Guides & Tutorials** | `/guides` | Step-by-step instructions | [guide-template](templates/guide-template.md) |
| **Feature Specs** | `/features` | Feature implementation details | [feature-template](templates/feature-template.md) |
| **Team Standards** | `/rules` | Policies and conventions | N/A |
| **Meeting Notes** | Varies | Meeting records | [meeting-notes-template](templates/meeting-notes-template.md) |

## 🎯 Quick Links by Role

### Team Lead
- [Rules & Guidelines](rules/README.md) - Team policies
- [Project Index](projects/README.md) - All projects overview
- [Meeting Notes Template](templates/meeting-notes-template.md) - Recording meetings

### Developer
- [Git Workflow](guides/git-workflow.md) - Version control
- [Project Documentation](projects/README.md) - Project details
- [Feature Documentation](features/README.md) - Feature specs

### New Member
- [Onboarding Guide](guides/onboarding.md) - Start here
- [Contributing Guide](CONTRIBUTING.md) - How to contribute
- [Documentation Standards](rules/documentation-standards.md) - Writing docs

### Documentation Writer
- [Contributing Guide](CONTRIBUTING.md) - Contribution process
- [Templates](templates/README.md) - All templates
- [Markdown Cheatsheet](templates/markdown-cheatsheet.md) - Syntax reference

## 🔍 Finding What You Need

### By Task
- **Starting a new project**: Use [project template](templates/project-template/)
- **Writing a tutorial**: Use [guide template](templates/guide-template.md)
- **Documenting a feature**: Use [feature template](templates/feature-template.md)
- **Learning the workflow**: Read [Git workflow guide](guides/git-workflow.md)
- **Onboarding someone**: Share [onboarding guide](guides/onboarding.md)

### By Question
- **How do I...?** → [Guides](guides/README.md)
- **What is...?** → [Features](features/README.md) or [Projects](projects/README.md)
- **What are the rules for...?** → [Rules](rules/README.md)
- **Where's the template for...?** → [Templates](templates/README.md)

## 📊 Documentation Lifecycle

```
1. PLAN
   ↓
   Identify documentation need
   Choose appropriate type/template
   
2. WRITE
   ↓
   Use template
   Follow documentation standards
   Include examples and code
   
3. REVIEW
   ↓
   Self-review checklist
   Peer review via PR
   
4. PUBLISH
   ↓
   Merge to main
   Update index files
   
5. MAINTAIN
   ↓
   Update when code changes
   Review periodically
   Archive when obsolete
```

## 🎨 Visual Legend

📁 Directory/Folder  
📄 Document/File  
🚀 Quick Start  
📚 Learning Resource  
⚙️ Configuration  
✅ Checklist/Task  
🗺️ Navigation  
🔍 Search/Find  

## 🤔 Still Lost?

1. Check the [main README](README.md) for overview
2. Browse the [Templates](templates/README.md) section
3. Read the [Contributing Guide](CONTRIBUTING.md)
4. Ask in team communication channels
5. Open an issue for clarification

---

*This map provides a visual overview of the documentation structure. For detailed information, explore the linked sections.*

# Markdown Cheatsheet

Quick reference guide for markdown syntax used in DTRG documentation.

## Headers

```markdown
# H1 - Main Title
## H2 - Section
### H3 - Subsection
#### H4 - Sub-subsection
##### H5 - Minor heading
###### H6 - Smallest heading
```

## Text Formatting

```markdown
**Bold text**
*Italic text*
***Bold and italic***
~~Strikethrough~~
`Inline code`
```

**Bold text**  
*Italic text*  
***Bold and italic***  
~~Strikethrough~~  
`Inline code`

## Lists

### Unordered Lists
```markdown
- Item 1
- Item 2
  - Nested item 2.1
  - Nested item 2.2
- Item 3
```

### Ordered Lists
```markdown
1. First item
2. Second item
3. Third item
   1. Nested item 3.1
   2. Nested item 3.2
```

### Task Lists
```markdown
- [x] Completed task
- [ ] Incomplete task
- [ ] Another incomplete task
```

## Links

```markdown
[Link text](https://example.com)
[Link with title](https://example.com "Link title")
[Relative link to file](../guides/guide-name.md)
[Link to section](#section-name)
```

## Images

```markdown
![Alt text](image-url.png)
![Alt text with title](image-url.png "Image title")
```

## Code

### Inline Code
```markdown
Use `code` for inline code snippets.
```

### Code Blocks

````markdown
```python
def hello_world():
    print("Hello, World!")
```
````

Common languages: `python`, `javascript`, `bash`, `json`, `yaml`, `sql`, `markdown`

## Blockquotes

```markdown
> This is a blockquote
> It can span multiple lines
>
> And have multiple paragraphs
```

> This is a blockquote

## Tables

```markdown
| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Row 1    | Data     | Data     |
| Row 2    | Data     | Data     |

| Left align | Center align | Right align |
|:-----------|:------------:|------------:|
| Left       | Center       | Right       |
```

| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Row 1    | Data     | Data     |
| Row 2    | Data     | Data     |

## Horizontal Rule

```markdown
---
or
***
or
___
```

---

## Escaping Characters

```markdown
\* Escaped asterisk
\# Escaped hash
\[ Escaped bracket
```

## Emoji (GitHub-flavored markdown)

```markdown
:rocket: :sparkles: :books: :white_check_mark: :x: :warning:
```

🚀 ✨ 📚 ✅ ❌ ⚠️

### Common Emoji for Documentation

- ✅ `:white_check_mark:` - Complete/Success
- ❌ `:x:` - Failed/Error
- ⚠️ `:warning:` - Warning
- 🚧 `:construction:` - In Progress
- 📝 `:memo:` - Documentation
- 🚀 `:rocket:` - Deployment/Launch
- 🐛 `:bug:` - Bug
- ✨ `:sparkles:` - New Feature
- 🔧 `:wrench:` - Configuration
- 📊 `:bar_chart:` - Data/Analytics

## Collapsible Sections

```markdown
<details>
<summary>Click to expand</summary>

Hidden content goes here.

Can include **formatting**, code, etc.

</details>
```

<details>
<summary>Click to expand</summary>

Hidden content goes here.

</details>

## Comments

```markdown
<!-- This is a comment that won't be visible in the rendered output -->
```

## Best Practices for DTRG Docs

1. **Use descriptive link text**: Instead of "click here", use "see the setup guide"
2. **Add language to code blocks**: Always specify the language for syntax highlighting
3. **Use relative links**: For internal documentation, use relative paths
4. **Include alt text for images**: Describe what the image shows
5. **Keep lines reasonable length**: Aim for 80-120 characters per line for readability
6. **Use headers hierarchically**: Don't skip heading levels (H1 → H3)
7. **Add blank lines**: Around code blocks, lists, and between sections for clarity

## Additional Resources

- [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/)
- [CommonMark Spec](https://commonmark.org/)
- [GitHub-Flavored Markdown Spec](https://github.github.com/gfm/)

---

*Keep this cheatsheet handy when writing DTRG documentation!*

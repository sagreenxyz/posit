---
layout: ../../layouts/Layout.astro
title: Getting Started
---

# Getting Started

Welcome to Posit! This guide will help you get started with creating and managing your markdown documentation.

## What is Posit?

Posit is a static documentation site built with Astro, optimized for hosting markdown documents with a clean, professional appearance.

## Creating New Pages

To create a new documentation page:

1. Create a new `.md` or `.astro` file in the `src/pages` directory
2. Add frontmatter with your page metadata
3. Write your content in Markdown

### Example Markdown Page

```markdown
---
layout: ../../layouts/Layout.astro
title: My New Page
---

# My Page Title

Your content goes here!
```

## Markdown Features

Posit supports all standard markdown features:

### Headers

Use `#` for headers (H1 through H6):

```
# H1 Header
## H2 Header
### H3 Header
```

### Text Formatting

- **Bold text** using `**bold**`
- *Italic text* using `*italic*`
- ***Bold and italic*** using `***both***`
- `Inline code` using backticks

### Lists

Unordered lists:
- Item 1
- Item 2
  - Nested item
  - Another nested item

Ordered lists:
1. First item
2. Second item
3. Third item

### Links

Create links using `[link text](URL)`:

[Visit Astro](https://astro.build)

### Code Blocks

Use triple backticks for code blocks:

```javascript
function hello() {
  console.log("Hello, world!");
}
```

```python
def greet(name):
    print(f"Hello, {name}!")
```

### Blockquotes

> This is a blockquote.
> It can span multiple lines.

### Tables

| Feature | Status |
|---------|--------|
| Markdown | ✅ Supported |
| Syntax Highlighting | ✅ Supported |
| Responsive Design | ✅ Supported |

## Project Structure

```
posit/
├── src/
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       ├── index.astro
│       ├── about.md
│       └── docs/
│           ├── getting-started.md
│           └── features.md
├── public/
├── astro.config.mjs
└── package.json
```

## Development

To run the development server:

```bash
npm run dev
```

To build for production:

```bash
npm run build
```

To preview the production build:

```bash
npm run preview
```

## Next Steps

- Explore the [Features](./features/) page to learn more
- Check out the [About](../about/) page
- Start creating your own documentation!

---
layout: ../../layouts/Layout.astro
title: Features
---

# Features

Posit comes with a rich set of features designed to make documentation hosting simple and elegant.

## Core Features

### 📝 Markdown Support

Write your content in plain Markdown with full support for:

- Headers (H1-H6)
- Lists (ordered and unordered)
- Links and images
- Code blocks with syntax highlighting
- Tables
- Blockquotes
- And more!

### 🚀 Built with Astro

Astro provides:

- **Lightning-fast performance**: Static site generation means your pages load instantly
- **Zero JavaScript by default**: Only ship what you need
- **SEO-friendly**: Clean HTML output optimized for search engines
- **Modern tooling**: Built on Vite for fast development

### 🎨 Clean Design

- Professional and readable typography
- Responsive layout that works on all devices
- Consistent styling across all pages
- Optimized for readability

### 🌙 Syntax Highlighting

Code blocks are automatically highlighted with the GitHub Dark theme:

```javascript
// JavaScript example
const greeting = (name) => {
  return `Hello, ${name}!`;
};

console.log(greeting('World'));
```

```python
# Python example
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)

print(fibonacci(10))
```

```typescript
// TypeScript example
interface User {
  name: string;
  age: number;
}

function greetUser(user: User): string {
  return `Hello, ${user.name}!`;
}
```

## Navigation

Easy navigation between pages with:
- Top navigation bar
- Linked pages throughout the documentation
- Consistent URL structure

## Customization

The site is easy to customize:

- **Layouts**: Modify `src/layouts/Layout.astro` to change the overall design
- **Styles**: Update the CSS in the layout file
- **Navigation**: Edit the navigation links in the layout
- **Configuration**: Adjust settings in `astro.config.mjs`

## Performance

Astro's static generation ensures:

- **Fast load times**: Pre-rendered HTML pages
- **Minimal bandwidth**: Only essential resources are loaded
- **Great Core Web Vitals**: Optimized for Google's performance metrics

## Developer Experience

### Hot Reload

The development server includes hot module replacement (HMR) for instant updates as you edit.

### Type Safety

TypeScript support is built-in for type-safe development.

### Simple Structure

Clear project organization makes it easy to find and edit content.

## Production Ready

Build optimized production sites with:

```bash
npm run build
```

The output in the `dist/` folder is ready to deploy to any static hosting service:

- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages
- Any static file server

## Future Enhancements

Potential additions could include:

- [ ] Dark mode toggle
- [ ] Search functionality
- [ ] Table of contents for long pages
- [ ] Multiple theme options
- [ ] RSS feed for updates
- [ ] Pagination for large document sets

---

Ready to get started? Check out the [Getting Started guide](./getting-started/)!

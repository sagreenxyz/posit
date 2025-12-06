# Posit

A modern documentation website built with [Astro](https://astro.build) for hosting and displaying markdown documents.

## Features

- 📝 Write content in Markdown
- 🚀 Fast static site generation with Astro
- 🎨 Clean and readable design
- 📱 Responsive layout
- 🌙 Syntax highlighting for code blocks
- ⚡ Zero JavaScript by default
- 🔧 Easy to customize

## Getting Started

### Prerequisites

- Node.js 18 or higher
- npm (or yarn/pnpm)

### Installation

1. Clone this repository:
```bash
git clone https://github.com/sagreenxyz/posit.git
cd posit
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and visit `http://localhost:4321`

## Development

- **Start dev server**: `npm run dev`
- **Build for production**: `npm run build`
- **Preview production build**: `npm run preview`

## Project Structure

```
posit/
├── src/
│   ├── layouts/
│   │   └── Layout.astro       # Main layout template
│   └── pages/
│       ├── index.astro         # Homepage
│       ├── about.md            # About page
│       └── docs/
│           ├── getting-started.md
│           └── features.md
├── public/                     # Static assets
├── astro.config.mjs           # Astro configuration
├── package.json
└── tsconfig.json
```

## Adding New Pages

To add a new markdown document:

1. Create a new `.md` file in `src/pages/` or a subdirectory
2. Add frontmatter at the top:

```markdown
---
layout: ../layouts/Layout.astro
title: Your Page Title
---

# Your Page Title

Your content here...
```

3. The page will be automatically available at the corresponding URL

## Customization

### Styling

Edit the CSS in `src/layouts/Layout.astro` to customize the appearance.

### Navigation

Update the navigation links in `src/layouts/Layout.astro` (look for the `<nav>` section).

### Configuration

Modify `astro.config.mjs` to change Astro settings, including markdown configuration.

## Deployment

### GitHub Pages (Recommended)

This site is configured to automatically deploy to GitHub Pages. 

#### Setup Steps:

1. **Enable GitHub Pages in your repository:**
   - Go to your repository on GitHub
   - Navigate to **Settings** → **Pages**
   - Under **Source**, select **GitHub Actions**

2. **Push to the main branch:**
   - The GitHub Actions workflow (`.github/workflows/deploy.yml`) will automatically build and deploy your site
   - Your site will be available at `https://sagreenxyz.github.io/posit`

3. **Monitor the deployment:**
   - Go to the **Actions** tab in your repository to see the deployment progress
   - Once complete, your site will be live!

#### Manual Deployment

Build the site for production:

```bash
npm run build
```

The static site will be generated in the `dist/` directory. Deploy this folder to any static hosting service:

- **Netlify**: Connect your repository and set build command to `npm run build`
- **Vercel**: Import your repository and deploy
- **Cloudflare Pages**: Connect repository with build command `npm run build`

## Technologies Used

- [Astro](https://astro.build) - Web framework
- [TypeScript](https://www.typescriptlang.org/) - Type safety
- Markdown - Content format

## License

ISC

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

# Fictional Lamp - MkDocs Website

A modern, responsive blog site built with MkDocs and Material theme, featuring gradient colors, light/dark mode, and accessibility features.

## 🚀 Quick Start

### Installation

```bash
# Install dependencies
pip install -r requirements.txt
```

### Development

```bash
# Start development server with live reload
mkdocs serve

# The site will be available at http://127.0.0.1:8000
```

### Build

```bash
# Build the static site
mkdocs build --strict

# Output will be in the 'site' directory
```

## 📋 Features

- ✨ **Modern Design** - Built with MkDocs Material theme
- 🎨 **Gradient Theme** - Beautiful purple gradient color scheme
- 🌓 **Light/Dark Mode** - Toggle between themes with user preference detection
- 📱 **Fully Responsive** - Optimized for mobile, tablet, and desktop
- ♿ **Accessible** - WCAG compliant with ARIA labels and keyboard navigation
- 🖼️ **Hero Images** - Eye-catching SVG gradient hero images on each page
- 🔍 **Search** - Full-text search functionality included
- 📝 **Blog** - Ready-to-use blog structure with sample posts

## 📁 Project Structure

```
fictional-lamp/
├── docs/                           # Source content
│   ├── assets/
│   │   └── images/                 # Hero images (SVG)
│   ├── blog/
│   │   ├── index.md                # Blog landing page
│   │   └── posts/                  # Blog post articles
│   ├── stylesheets/
│   │   └── extra.css               # Custom styling
│   ├── index.md                    # Home page
│   └── contact.md                  # Contact page
├── .github/workflows/
│   └── deploy.yml                  # GitHub Pages deployment
├── mkdocs.yml                      # MkDocs configuration
├── requirements.txt                # Python dependencies
└── staticwebapp.config.json        # Azure Static Web Apps config
```

## 🎨 Customization

### Color Theme

The gradient color scheme is defined in `docs/stylesheets/extra.css`:

```css
:root {
  --gradient-primary: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  --gradient-secondary: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
  --gradient-accent: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
}
```

### Adding New Pages

1. Create a new `.md` file in the `docs/` directory
2. Add the page to the `nav` section in `mkdocs.yml`
3. Optionally add a hero image in `docs/assets/images/`

### Adding Blog Posts

1. Create a new `.md` file in `docs/blog/posts/`
2. Add a link to the post in `docs/blog/index.md`
3. Include metadata (title, date, author, category) in the post

## 🚀 Deployment

### GitHub Pages

The site automatically deploys to GitHub Pages when you push to the `main` branch.

1. Enable GitHub Pages in repository settings
2. Set the source to "GitHub Actions"
3. Push changes to trigger the workflow

The deployment workflow is in `.github/workflows/deploy.yml`.

### Azure Static Web Apps

1. Build the site: `mkdocs build`
2. Deploy the `site/` directory to Azure Static Web Apps
3. The `staticwebapp.config.json` contains the routing configuration

See `AZURE_DEPLOYMENT.md` for detailed instructions.

## ♿ Accessibility

The site follows WCAG guidelines and includes:

- Semantic HTML structure
- ARIA labels for screen readers
- Keyboard navigation support
- Proper focus states
- High contrast ratios
- Alt text for images

## 📝 Content Guidelines

### Writing Blog Posts

Each blog post should include:

- Clear title and heading structure
- Publication date and author
- Category tags
- Descriptive content with proper formatting
- Links back to the blog index

### Maintaining Consistency

- Use the same gradient colors throughout
- Include hero images on major pages
- Follow the established card design for features
- Maintain accessible markup patterns

## 🛠️ Technologies

- [MkDocs](https://www.mkdocs.org/) - Static site generator
- [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) - Theme
- [Python Markdown](https://python-markdown.github.io/) - Content processing
- [GitHub Actions](https://github.com/features/actions) - CI/CD

## 📄 License

See [LICENSE](LICENSE) file for details.

## 👤 Author

Sachin Sinha - [@sinhasachin](https://github.com/sinhasachin)

---

*Built with ❤️ using MkDocs and Material theme*

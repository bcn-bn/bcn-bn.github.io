# BCN Babylab Network Website

This is the website for the BCN Babylab Network built with [Quarto](https://quarto.org).

## Project Structure

```
.
├── _quarto.yml                    # Main Quarto configuration
├── index.qmd                      # Home page
├── about.qmd                      # About Us page
├── contact.qmd                    # Contact page
├── events/
│   ├── index.qmd                  # Events blog index
│   └── posts/
│       └── welcome.qmd            # Sample event post
├── styles.css                     # Custom styling
├── .gitignore                     # Git ignore patterns
└── README.md                      # This file
```

## Getting Started

### Prerequisites

- [Quarto](https://quarto.org/docs/get-started/) (v1.3 or later)

### Installation

1. Clone the repository
2. Install Quarto from https://quarto.org/docs/get-started/

### Development

To preview the website locally:

```bash
quarto preview
```

This will open your default browser and show a live preview of the site. Changes to files will automatically refresh.

To render the static website:

```bash
quarto render
```

The rendered site will be in the `_site/` directory.

## Adding Content

### Creating a New Event

To add a new event to the blog:

1. Create a new `.qmd` file in `events/posts/`
2. Add frontmatter with metadata:

```yaml
---
title: "Event Title"
date: "2026-06-15"
categories: [workshop, seminar]
---
```

3. Write the event content in Markdown/Quarto format
4. The event will automatically appear in the Events listing

Example event file: `events/posts/welcome.qmd`

### Editing Pages

The main pages are:

- **Home** (`index.qmd`)
- **About Us** (`about.qmd`)
- **Contact** (`contact.qmd`)
- **Events** (`events/index.qmd`)

Simply edit the `.qmd` files to update content.

## Customization

### Branding

Edit `styles.css` to customize colors:

- `--primary-color`: Main brand color (default: #0066cc - blue)
- `--secondary-color`: Accent color (default: #ff9900 - orange)

### Navigation

Edit `_quarto.yml` to modify the navigation bar, footer, and website title.

### Theme

Change the theme in `_quarto.yml`:

```yaml
format:
  html:
    theme: cosmo  # Other options: default, cerulean, journal, etc.
```

## Deployment

### GitHub Pages

The site is configured to deploy to GitHub Pages. To enable:

1. Go to repository Settings → Pages
2. Set "Build and deployment" source to "GitHub Actions"
3. Create a `.github/workflows/publish.yml` workflow to build and deploy

### Manual Deployment

```bash
quarto publish gh-pages
```

## Resources

- [Quarto Documentation](https://quarto.org)
- [Quarto Website Guide](https://quarto.org/docs/websites/)
- [Quarto Blog Setup](https://quarto.org/docs/websites/website-blog.html)

## Contributing

We welcome contributions! To contribute:

1. Create a new branch for your changes
2. Make your edits
3. Submit a pull request with a description of changes

## License

[Add license information here]

## Contact

For questions or suggestions, please contact: [info@bcnbabylabnetwork.org](mailto:info@bcnbabylabnetwork.org)

---

*Built with ❤️ for the BCN Babylab Network community*

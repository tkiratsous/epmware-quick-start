# EPMware Quick Start Guide - MkDocs Site

## Overview

This is the MkDocs source for the EPMware Quick Start Guide. The site provides step-by-step instructions for configuring your first EPMware application.

## Structure

```
quick-start-guide/
├── mkdocs.yml                 # MkDocs configuration file
├── docs/                       # Documentation source files
│   ├── index.md               # Home page
│   ├── assets/
│   │   ├── css/
│   │   │   └── custom.css    # Custom styling
│   │   └── images/            # Image placeholders
│   ├── getting-started/       # Getting started section
│   ├── configuration/         # Configuration guide
│   ├── security/              # Security setup
│   ├── global-settings/       # Global settings configuration
│   ├── services/              # Services management
│   ├── workflow/              # Workflow configuration
│   ├── deployment/            # Deployment setup
│   └── reference/             # Reference documentation
└── README.md                  # This file
```

## Prerequisites

To build and serve this documentation, you need:

- Python 3.7 or higher
- pip (Python package manager)

## Installation

1. Install MkDocs and the Material theme:

```bash
pip install mkdocs mkdocs-material mkdocs-glightbox
```

## Building the Documentation

### Serve Locally (Development)

To preview the documentation locally with live reload:

```bash
cd quick-start-guide
mkdocs serve
```

The site will be available at: http://localhost:8000

### Build Static Site

To build the static HTML site:

```bash
mkdocs build
```

The built site will be in the `site/` directory.

### Deploy to GitHub Pages

If hosting on GitHub Pages:

```bash
mkdocs gh-deploy
```

## Customization

### Adding Images

Replace the placeholder image files in `docs/assets/images/` with actual screenshots. Supported formats:
- PNG (recommended)
- JPG/JPEG
- GIF
- SVG

### Modifying Styles

Edit `docs/assets/css/custom.css` to customize the appearance. The current CSS includes:
- EPMware brand colors
- Custom admonitions
- Print-friendly styles
- Mobile optimizations

### Adding Content

1. Create new `.md` files in the appropriate directory
2. Update `mkdocs.yml` navigation section
3. Follow the existing content structure for consistency

## Content Guidelines

### Markdown Features

The site supports:
- Standard Markdown syntax
- Tables
- Admonitions (notes, warnings, tips)
- Code blocks with syntax highlighting
- Footnotes
- Image galleries (via glightbox plugin)

### Admonition Examples

```markdown
!!! note "Important Note"
    This is a note with custom styling.

!!! warning "Caution"
    This is a warning message.

!!! tip "Best Practice"
    This is a helpful tip.
```

## Navigation

The navigation is configured in `mkdocs.yml`. Each main section includes:
- An index.md file as the section landing page
- Anchor links to subsections for easy navigation
- Related topics links at the bottom of each page

## Support

For questions or issues:
- Email: support@epmware.com
- Phone: 408-614-0442
- Documentation: https://docs.epmware.com

## License

© 2025 EPMware, Inc. All rights reserved.

## Version

- Document Version: 2.6
- Last Updated: November 2020 (Content)
- MkDocs Structure: January 2025

# Kupia Audit Arsenal 🛡️

A comprehensive knowledge hub for Web3 security auditors, containing curated resources, audit methodologies, and DeFi concepts.

## About This Repository

This repository hosts the Kupia Audit Arsenal documentation site built with MkDocs. It serves as a central knowledge base for smart contract auditors, containing:

- 🔍 **Audit Methodologies**: Comprehensive notes from Owen of GuardianAudit's Web3 Security 101 videos
- 💰 **DeFi Concepts**: Technical breakdowns from Finematics explaining protocol mechanics
- 🎙️ **Podcast Insights**: Key security lessons from Andy Li, Johnny Time, and Proof Of Podcast

## Content Overview

- **Audit Section**: Learn how to think like a top-tier auditor with breakdowns of common vulnerabilities
- **DeFi Concepts**: Understand the underlying mechanics of various DeFi protocols
- **Podcast Notes**: Insights directly from security experts and researchers

## Getting Started

### Prerequisites

- Python 3.x
- pip

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/KupiaSec/kupia-audit-arsenal.git
   cd kupia-audit-arsenal
   ```

2. Create a virtual environment:
   ```bash
   python -m virtualenv venv
   ```

3. Activate the virtual environment:
   ```bash
   # On Windows
   venv\Scripts\activate
   # On macOS/Linux
   source venv/bin/activate
   ```

4. Install MkDocs and required plugins:
   ```bash
   pip install mkdocs mkdocs-material
   ```
   Refer to [MkDocs documentation](https://www.mkdocs.org/user-guide/installation/) for more details.

## Development

To run the documentation site locally:

```bash
mkdocs serve
```

This will start a development server at http://127.0.0.1:8000/

## Adding Content

### Adding a New Page

1. Create a new Markdown file in the appropriate directory under `docs/`
2. Add the page to the navigation in `mkdocs.yml`:

```yaml
nav:
  - Home: index.md
  - Audit:
    - audit/vulnerability-types.md
    - audit/your-new-page.md
  # Other sections...
```

## Deployment

### GitHub Pages

To deploy to GitHub Pages:

```bash
mkdocs gh-deploy
```

This command builds the site and pushes it to the `gh-pages` branch of your repository.

### Custom Hosting

To build the site for custom hosting:

```bash
mkdocs build
```

The built site will be in the `site/` directory, which you can then deploy to your hosting provider.


## License

This repository is only for educational purposes. All the rights belong to the origial content owners.

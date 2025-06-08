# alican.de - Personal Website

Automatically created through Hugo and GitHub Actions. This is my personal website built with Hugo and the Stack theme, deployed via GitHub Pages.

## 🚀 Quick Start

To run your Hugo site locally, follow these steps:

### Prerequisites

1. **Install Hugo** if you haven't already:
   ```bash
   brew install hugo
   ```
   Or download from [Hugo's official site](https://gohugo.io/getting-started/installing/)

### Running Locally

2. **Initialize and update the theme submodule** (since you're using the Stack theme as a submodule):
   ```bash
   git submodule update --init --recursive
   ```

3. **Start the Hugo development server**:
   ```bash
   hugo server
   ```

This will start a local development server at `http://localhost:1313` and automatically reload when you make changes to your content.

### Additional Options

You can also run with additional options:
- `hugo server -D` to include draft content
- `hugo server --bind 0.0.0.0` to make it accessible from other devices on your network

## 📁 Project Structure

```
├── config.yaml          # Hugo configuration
├── content/             # All content files
│   ├── docs/           # Documentation pages
│   ├── page/           # Static pages
│   ├── post/           # Blog posts
│   └── categories/     # Category definitions
├── layouts/            # Custom layout overrides
├── assets/             # Assets (SCSS, images, icons)
├── static/             # Static files
└── themes/stack/       # Hugo Theme Stack (submodule)
```

## 🎨 Theme

This site uses the [Hugo Theme Stack](https://github.com/CaiJimmy/hugo-theme-stack), which is configured in the [`config.yaml`](config.yaml) file. The theme provides:
- Modern card-style design
- Search functionality
- Categories and tags
- Dark/light mode toggle
- Mobile-responsive layout

## 🔧 Deployment

The site is automatically deployed via GitHub Actions when you push to the master branch. See [`.github/workflows/main.yml`](.github/workflows/main.yml) for the deployment configuration.

## 📝 Content Management

Content is written in Markdown and organized in the `content/` directory:
- **Blog posts**: `content/post/`
- **Documentation**: `content/docs/`
- **Static pages**: `content/page/`
- **Categories**: `content/categories/`

## 🌐 Live Site

Visit the live site at: [https://alican.de](https://alican.de)

## 📄 License

Content is licensed under the terms specified in individual posts. The Hugo Theme Stack is licensed under GPL v3.0.
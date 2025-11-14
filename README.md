# TE Connectivity Demo Site

A modern, responsive Jekyll-based website showcasing TE Connectivity Ltd., a global leader in connectivity and sensor solutions.

## 🌐 Live Demo

Visit the live site: [https://gowthame123.github.io/my_demo_site](https://gowthame123.github.io/my_demo_site)

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technology Stack](#technology-stack)
- [Getting Started](#getting-started)
- [Customization](#customization)
- [Pages](#pages)
- [Deployment](#deployment)
- [License](#license)

## 📖 About

This is a professional website for TE Connectivity Ltd. (NYSE: TEL), built with Jekyll and hosted on GitHub Pages. The site provides an overview of the company's mission, history, products, and global presence.

TE Connectivity is an American-Irish technology company specializing in:
- High-performance connectors and sensors
- Power distribution and signal management
- Cable and wiring solutions
- Electronics for automotive, industrial, aerospace, and medical applications

## ✨ Features

- **Responsive Design**: Mobile-friendly layout using CSS Grid and Flexbox
- **Yellow Sidebar**: Eye-catching navigation with centered logo
- **Hero Section**: Compelling headline and company positioning
- **Fast Performance**: Static site generation with Jekyll
- **Easy Customization**: Simple Markdown and YAML configuration
- **SEO-Friendly**: Semantic HTML structure
- **Dark/Light Compatibility**: Works across different color schemes

## 📁 Project Structure

```
my_demo_site/
├── _config.yml              # Jekyll configuration
├── _includes/
│   ├── head.html           # Meta tags and CSS links
│   └── sidebar.html        # Navigation and logo
├── _layouts/
│   ├── default.html        # Main layout wrapper
│   ├── page.html           # Page layout
│   └── post.html           # Blog post layout
├── _posts/                 # Blog posts (optional)
├── public/
│   └── css/
│       ├── poole.css       # Base styles
│       ├── hyde.css        # Theme styles
│       └── syntax.css      # Code highlighting
├── images/
│   └── logo.png            # Logo image
├── index.html              # Home page
├── about.md                # About page
├── Gemfile                 # Ruby dependencies
└── README.md               # This file
```

## 🛠 Technology Stack

- **Static Site Generator**: Jekyll 4.3.4
- **Templating**: Liquid
- **Styling**: CSS3
- **Markdown Processor**: Kramdown
- **Syntax Highlighting**: Rouge
- **Hosting**: GitHub Pages
- **Version Control**: Git

### Dependencies

- jekyll (~> 4.3.4)
- jekyll-paginate
- jekyll-gist
- kramdown
- rouge (syntax highlighter)
- wdm (Windows file monitoring)

## 🚀 Getting Started

### Prerequisites

- Ruby 3.0+ installed
- Git installed
- GitHub account

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/Gowthame123/my_demo_site.git
   cd my_demo_site
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Run the local server**
   ```bash
   bundle exec jekyll serve --trace
   ```

4. **View in browser**
   Open `http://127.0.0.1:4000/my_demo_site/` in your browser

### Making Changes

- Edit Markdown files (`.md`) for content
- Edit CSS in `public/css/` for styling
- Edit HTML in `_includes/` or `_layouts/` for structure
- Changes auto-reload with `jekyll serve`

## ⚙️ Customization

### Site Configuration

Edit `_config.yml` to customize:

```yaml
title:            "TE Connectivity"      # Site title
tagline:          "Your tagline"        # Subtitle
description:      "Description.."       # Meta description
baseurl:          "/my_demo_site"       # Project path on GitHub Pages
```

### Sidebar Logo

Replace `images/logo.png` with your own logo (recommended size: 150x150px or larger).

### Color Scheme

Modify `public/css/hyde.css` to change:
- Background color: `.sidebar { background-color: #FFD700; }`
- Text color: `.sidebar { color: #000; }`
- Logo size: `.sidebar-logo { width: 150px; }`

### Navigation Links

Edit `_includes/sidebar.html` to add/remove pages. Pages automatically appear in navigation if they have:
```yaml
layout: page
title: "Page Title"
```

## 📄 Pages

### Home (`index.html`)

Features:
- Hero section with company headline
- "Precision in Every Connection" section
- "Applications That Matter" section highlighting key industries
- "Global Scale, Local Impact" section

### About (`about.md`)

Includes:
- Company history (1941–present)
- Global footprint and team size
- Product portfolio table
- Commitment to sustainability
- Innovation and R&D investment

## 🌍 Deployment

### GitHub Pages Setup

1. Push code to GitHub repository: `git push origin master`
2. Go to repository **Settings** → **Pages**
3. Select **Deploy from a branch** → **master** → **/ (root)**
4. Site builds automatically and appears at `https://gowthame123.github.io/my_demo_site`

### Build Time

GitHub typically builds within 1-2 minutes after each push. Check build status in the **Actions** tab.

## 🔧 Troubleshooting

### Layout/CSS not appearing

**Issue**: Assets (CSS, images) are 404s

**Solution**: Ensure `baseurl: "/my_demo_site"` is set correctly in `_config.yml`

### Logo not displaying

**Issue**: Image returns 404

**Solution**: 
- Confirm `images/logo.png` exists in the repository
- Check file is committed and pushed to GitHub
- Clear browser cache (Ctrl+F5)

### Navigation links broken

**Issue**: Links return 404 or don't navigate

**Solution**: 
- Use `relative_url` filter in links: `href="{{ path | relative_url }}"`
- Ensure pages have correct front-matter with `layout` and `title`

## 📝 License

This project is open source and available under the MIT License. See LICENSE.md for details.

## 👤 Author

**Gowthame123**

- GitHub: [@Gowthame123](https://github.com/Gowthame123)
- Repository: [my_demo_site](https://github.com/Gowthame123/my_demo_site)

## 🎯 Future Enhancements

- Blog section with posts
- Product catalog pages
- Contact form
- Search functionality
- Dark mode toggle
- Multi-language support

## 📞 Support

For questions or issues:
1. Check the [Jekyll documentation](https://jekyllrb.com/docs/)
2. Review [GitHub Pages documentation](https://docs.github.com/en/pages)
3. Open an issue in the repository

---

**Built with ❤️ using Jekyll and hosted on GitHub Pages**

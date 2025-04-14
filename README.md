# AI Tools Directory 🤖

> The ultimate curated collection of AI tools and resources in a beautiful, searchable directory.

[![Netlify Status](https://api.netlify.com/api/v1/badges/YOUR-NETLIFY-ID/deploy-status)](https://app.netlify.com/sites/your-site/deploys)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Support & Resources](#support--resources)

## Overview

AI Tools is a responsive directory website showcasing artificial intelligence tools and resources in a clean, three-column grid layout. The site features category filtering, search functionality, and a modern design optimized for user experience.

## Features

- 🔍 Instant search functionality
- 📱 Responsive 3-column grid layout
- 🏷️ Category-based filtering
- 🎯 SEO optimized
- 🚀 Fast loading times
- 💻 Easy customization
- 🌓 Dark/Light mode toggle

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- Git

### Local Development
```bash
# Clone the repository
git clone https://github.com/yourusername/ai-tools-directory.git

# Navigate to project directory
cd ai-tools-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
ai-tools-directory/
├── src/
│   ├── components/
│   │   ├── Card.js
│   │   ├── Grid.js
│   │   └── Search.js
│   ├── data/
│   │   └── tools.json
│   ├── styles/
│   │   └── main.css
│   └── pages/
├── public/
│   └── images/
├── package.json
└── README.md
```

## Customization Guide

### Adding Directory Items

Edit `src/data/tools.json`:
```json
{
  "items": [
    {
      "id": "1",
      "name": "Tool Name",
      "description": "Tool description",
      "category": "Category",
      "url": "https://example.com",
      "image": "/images/tool-image.png"
    }
  ]
}
```

### Modifying Categories

Edit `src/data/categories.js`:
```javascript
export const categories = [
  "AI Writing",
  "Image Generation",
  "Video Creation",
  "Code Assistant"
];
```

### Updating Hero Section

Modify `src/components/Hero.js`:
```jsx
<div className="hero">
  <h1>Your Custom Title</h1>
  <p>Your custom description text</p>
</div>
```

### Customizing Colors

Edit `src/styles/variables.css`:
```css
:root {
  --primary-color: #007bff;
  --secondary-color: #6c757d;
  --background-color: #ffffff;
  --text-color: #333333;
}
```

## Deployment

### Netlify Deployment
1. Connect your GitHub repository to Netlify
2. Configure build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
3. Click "Deploy"

### Vercel Deployment
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

## Custom Domain Setup

1. Purchase domain from your preferred registrar
2. Add domain in deployment platform:
   ```
   Custom domain: www.youraitools.com
   ```
3. Configure DNS settings:
   ```
   Type    Name    Value
   A       @       76.76.21.21
   CNAME   www     yoursite.netlify.app
   ```

## Troubleshooting

### Common Issues

**Build Failures**
```bash
# Clear cache and node modules
rm -rf node_modules
rm -rf .cache
npm install
```

**Image Loading Issues**
- Ensure images are in the correct format (PNG/JPG)
- Verify file paths in tools.json
- Check image optimization settings

## Support & Resources

- 📚 [Documentation Wiki](https://github.com/yourusername/ai-tools-directory/wiki)
- 🐛 [Issue Tracker](https://github.com/yourusername/ai-tools-directory/issues)
- 💬 [Community Discord](https://discord.gg/yourserver)
- 📧 [Support Email](mailto:support@aitools.com)

### Useful Links
- [Contribution Guidelines](CONTRIBUTING.md)
- [Code of Conduct](CODE_OF_CONDUCT.md)
- [License](LICENSE.md)

---

## License
MIT © [Your Name]
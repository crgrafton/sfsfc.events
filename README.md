# SF Street Fair Coalition Website

A modern, vibrant website for the San Francisco Street Fair Coalition, celebrating community, culture, and commerce.

## 🎨 Design Features

### Visual Design
- **Pride-Inspired Color Palette**: Custom CSS variables based on Pride colors
- **Modern Gradients**: Smooth gradient backgrounds and accent elements
- **Responsive Grid Layout**: Mobile-first design with Bootstrap 5.3.3
- **Smooth Animations**: Subtle fade-in effects and hover interactions
- **Accessible Typography**: Atkinson Hyperlegible font for improved readability

### Key Sections
1. **Hero Section**: Eye-catching gradient header with clear CTAs
2. **Image Gallery**: Hover-activated overlay gallery showcasing events
3. **About Section**: Feature cards with statistics and mission statement
4. **Values Section**: Icon-based presentation of core principles
5. **Members Section**: Showcase of member organizations with hover effects
6. **Contact Section**: Clean, centered contact card with prominent CTA

### Technical Features
- Sticky navigation with scroll effects
- Smooth scrolling to anchor links
- SEO-optimized meta tags
- Open Graph tags for social sharing
- Mobile-responsive design
- Custom 404 error page

## 🚀 Development

### Prerequisites
- Ruby 3.2+
- Jekyll
- Bundler

### Installation
```bash
bundle install
```

### Local Development
```bash
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`

### Building for Production
```bash
bundle exec jekyll build
```

## 📁 Project Structure

```
.
├── _config.yml           # Jekyll configuration
├── _layouts/
│   └── default.html      # Main layout template
├── assets/
│   └── main.scss         # Custom styles with Bootstrap
├── images/               # Image assets
├── index.html            # Main page content
├── 404.html              # Custom error page
└── README.md             # This file
```

## 🎨 Design System

### Color Variables
- `--sf-pride-red`: #E40303
- `--sf-pride-orange`: #FF8C00
- `--sf-pride-yellow`: #FFED00
- `--sf-pride-green`: #008026
- `--sf-pride-blue`: #24408E
- `--sf-pride-purple`: #732982

### Typography
- Primary Font: Atkinson Hyperlegible
- Display Font: Major Mono Display
- Fallback Fonts: Noto Sans, Noto Serif

### Key Components
- `.hero-section`: Gradient hero with animations
- `.image-gallery`: Grid-based gallery with hover overlays
- `.feature-card`: Hover-enabled content cards
- `.value-item`: Icon-based value presentations
- `.member-card`: Organization showcase cards

## 📝 Content Management

### Adding New Members
1. Add organization logo to `/images/`
2. Update the Members Section in `index.html`
3. Follow the existing `.member-card` structure

### Updating Content
- Main content is in `index.html`
- Styles are in `assets/main.scss`
- Site configuration in `_config.yml`

## 🔗 Important Links

- [Donate](https://donate.stripe.com/14kbLOfsh4GxguYfZ8)
- [Sign Up for Updates](https://forms.gle/BEXqSSFPR95cgWfK8)
- [Press Release](https://docs.google.com/document/d/145gsljCt7uH_elPjyLhbQAYK1a8IqkG-EJON93PgJBY/edit)

## 📧 Contact

Email: sfstreetfaircoalition@gmail.com

---

Built with ❤️ for the San Francisco community

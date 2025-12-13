# Cloudflare Pages Deployment Guide

## Build Settings for Cloudflare Pages

Use these settings in your Cloudflare Pages dashboard:

- **Build command:** `bundle exec jekyll build`
- **Build output directory:** `_site`
- **Root directory:** `/` (leave empty or use `/`)

### Environment Variables

Set these in Cloudflare Pages > Settings > Environment Variables:

```
JEKYLL_ENV=production
```

### Ruby Version

The site is configured to work with Ruby 3.2.2 (Cloudflare Pages default).

## Local Development

```bash
# Install dependencies
bundle install

# Build the site
bundle exec jekyll build

# Serve locally with live reload
bundle exec jekyll serve --livereload
```

Visit http://localhost:4000

## Key Changes for Cloudflare Deployment

1. **Bootstrap via CDN**: Using Bootstrap 5.3.3 from jsDelivr CDN instead of the gem to avoid Ruby version path issues
2. **Simplified Gemfile**: Removed bootstrap gem and unnecessary dependencies
3. **Compressed CSS**: Production builds use compressed CSS for better performance
4. **Standard gems included**: csv, logger, and base64 gems explicitly included for Ruby 3.4+ compatibility

## Troubleshooting

If the build fails on Cloudflare Pages:

1. Check that the build command is exactly: `bundle exec jekyll build`
2. Verify the output directory is: `_site`
3. Ensure Ruby version is 3.2.2 or higher
4. Check the build logs for any missing gems

## Architecture

- **Framework**: Jekyll 4.3.3
- **CSS Framework**: Bootstrap 5.3.3 (CDN)
- **Deployment**: Cloudflare Pages
- **Custom CSS**: `/assets/main.scss` compiled to `/assets/main.css`

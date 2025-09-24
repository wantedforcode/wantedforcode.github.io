# WantedForCode Jekyll Site - AI Coding Instructions

## Project Overview
This is a Jekyll-based business portfolio website using the `raviriley/agency-jekyll-theme` remote theme. The site showcases WantedForCode's technology consulting services, portfolio projects, and team information.

## Architecture & Key Files

### Theme Structure
- **Remote Theme**: Uses `raviriley/agency-jekyll-theme` from GitHub (configured in `_config.yml`)
- **Content Data**: All site content is in `_data/sitetext.yml` (multilingual YAML structure)
- **Navigation**: Configured in `_data/navigation.yml` with section-based navigation
- **Portfolio**: Individual project files in `_portfolio/` directory with frontmatter metadata

### Critical Configuration Files
- `_config.yml`: Site settings, theme config, Formspree contact form integration
- `Gemfile`: Jekyll dependencies (minimal - relies heavily on remote theme)
- `_data/sitetext.yml`: All site text content organized by language (`en` default)
- `_data/navigation.yml`: Site navigation structure

## Development Workflow

### Local Development
```bash
# Install dependencies
bundle install

# Serve locally (with auto-reload)
bundle exec jekyll serve

# Access at http://localhost:4000
```

### Content Updates
- **Services/About/Contact**: Edit `_data/sitetext.yml` under respective sections
- **Portfolio Projects**: Add/edit `.md` files in `_portfolio/` with proper frontmatter
- **Team Members**: Update `team` section in `_data/sitetext.yml`
- **Site Branding**: Modify header, title, tagline in `_config.yml` and `_data/sitetext.yml`

## Project-Specific Patterns

### Portfolio Project Structure
Each project in `_portfolio/` follows this pattern:
```yaml
---
title: Project Name
subtitle: Brief description
image: assets/img/portfolio/project-image.jpg
alt: Accessibility description
caption:
  title: Short Title
  subtitle: Tech Stack
  thumbnail: assets/img/portfolio/thumb.jpg
---
```

### Content Localization
- All text uses the pattern `{{ site.data.sitetext[site.locale].section.key }}`
- Default locale is `en`, expandable for Spanish (`es`) and others
- Navigation follows same localization pattern in `navigation.yml`

### Asset Organization
- **Images**: `assets/img/` with subdirectories (`portfolio/`, `team/`, `clients/`)
- **Custom Styles**: `assets/css/custom-styles.css` for theme overrides
- **Logo**: Configured in `_config.yml` with path and height settings

## Integration Points
- **Contact Form**: Formspree integration via `formspree_form_path` in `_config.yml`
- **Analytics**: Google Analytics placeholder in `_config.yml`
- **Remote Theme**: GitHub-hosted theme updates automatically

## Common Tasks
- **Adding Portfolio Project**: Create new `.md` file in `_portfolio/` with proper frontmatter and assets
- **Updating Contact Info**: Modify `contact` section in `_data/sitetext.yml` and email in `_config.yml`
- **Styling Changes**: Add CSS rules to `assets/css/custom-styles.css`
- **Team Updates**: Edit `team` array in `_data/sitetext.yml`

## Deployment
Site is configured for GitHub Pages deployment with custom domain `wantedforcode.com` (see `CNAME` file).
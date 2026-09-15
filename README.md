# Survey Template

A modern, customizable survey template homepage built with Quarto, inspired by the [Real World Data Science](https://realworlddatascience.net/) design system.

## Features

- **Clean, Modern Design**: Professional layout with a cohesive visual identity
- **Responsive**: Works seamlessly on desktop, tablet, and mobile devices
- **Customizable**: Easy-to-modify colors, fonts, and layout
- **Built with Quarto**: Simple to build and deploy
- **Professional Typography**: Uses Oswald and Montserrat fonts

## Project Structure

```
survey_template/
├── _quarto.yml          # Quarto configuration
├── index.qmd            # Homepage
├── about.qmd            # About page
├── contact.qmd          # Contact page
├── rwds.css             # Main stylesheet (copied from RWDS)
├── rwds.scss            # SCSS configuration
├── README.md            # This file
└── .gitignore           # Git ignore rules
```

## Quick Start

1. **Install Quarto** (if you haven't already)
   - Download from https://quarto.org/docs/get-started/

2. **Preview the site locally**
   ```bash
   quarto preview
   ```
   The site will open at `http://localhost:5000`

3. **Customize for your needs**
   - Edit `_quarto.yml` to update site title, URLs, and navigation
   - Edit `index.qmd` to customize the homepage
   - Edit `rwds.css` to change colors and styling
   - Create additional `.qmd` files for new pages

4. **Build and publish**
   ```bash
   quarto render
   ```
   Deploy the `_site/` folder to your hosting provider

## Customization Guide

### Colors

The color scheme is defined in `rwds.css`. Key colors:

- **Primary Purple**: `#939bc9` - Used for links and accents
- **Black**: `#000000` - Text and borders
- **Light Background**: `#f0eeeb` - Page background
- **White**: `#ffffff` - Contrast

To change colors, find and replace these hex values in `rwds.css`.

### Typography

- **Headings**: Oswald font (imported from Google Fonts)
- **Body Text**: Montserrat font (imported from Google Fonts)

Change fonts in `rwds.css` by modifying the `@import` statement at the top.

### Navbar

Edit `_quarto.yml` to customize navigation:

```yaml
navbar:
  right:
    - text: "Page Name"
      href: page.qmd
```

## License

This template is based on the design system from [Real World Data Science](https://realworlddatascience.net/), used under their open-source license. See the RWDS repository for more details on their licensing.

## Resources

- [Quarto Documentation](https://quarto.org)
- [Real World Data Science](https://realworlddatascience.net/)
- [Quarto Websites Guide](https://quarto.org/docs/websites/)

## Support

For questions about Quarto, visit their [documentation](https://quarto.org/docs/get-started/).

For customization help, refer to the inline comments in the CSS and YAML files.

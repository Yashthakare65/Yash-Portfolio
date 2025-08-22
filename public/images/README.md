# Project Images

Place your project screenshots and cover images in this folder.

## Required Images

For the portfolio to work correctly, add these images:

1. **portfolio-cover.jpg** - Screenshot of your portfolio project
2. **cookie-delights-cover.jpg** - Screenshot of your cookie website project

## Image Specifications

- **Format**: JPG or PNG
- **Aspect Ratio**: 16:7 (recommended for project cards)
- **Size**: 800x350px or similar 16:7 ratio
- **Quality**: High quality, clear screenshots

## Adding New Projects

When adding new projects to `src/components/Projects.jsx`, make sure to:

1. Add the image file to this folder
2. Update the image path in the projects array
3. Use relative paths like `./images/filename.jpg`

## Fallback System

If images fail to load, the portfolio will automatically show:
- A gradient background with the project title
- An emoji icon (📱)
- The project name

This ensures the portfolio always looks good even without images.

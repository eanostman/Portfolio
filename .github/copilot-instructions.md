# Copilot Instructions for Portfolio Website

## Project Overview
- This is a static personal portfolio website for Ean Ostman, built with HTML, CSS, and Bootstrap 5.
- The site consists of three main pages: `index.html` (Home), `About.html` (About Me), and `Contact.html` (Contact).
- All pages share a consistent navigation bar and a responsive footer overlay with social links.
- Custom styles are defined in `style.css`, with support for both light and dark color schemes.

## Key Patterns & Conventions
- **Navigation and Footer:**
  - The navigation bar and footer are nearly identical across all pages. Update all HTML files for global navigation/footer changes.
  - Social icons use Bootstrap Icons via CDN.
- **Styling:**
  - Use `style.css` for all custom styles. It includes responsive and color-scheme-aware rules for the footer and navigation.
  - The `.main-content` class is used to add bottom padding to prevent content from being hidden behind the fixed footer.
- **Responsive Design:**
  - Bootstrap grid and utility classes are used for layout and responsiveness.
  - Media queries in `style.css` further refine mobile appearance.
- **Assets:**
  - Images (`programming.webp`, `ean headshot.png`) are referenced directly in HTML.
  - No build step or asset pipeline; all files are static and referenced by relative path.

## Developer Workflows
- **Previewing:**
  - Open `index.html` (or any page) directly in a browser for local preview.
  - No build, test, or deployment scripts are present; this is a pure static site.
- **Deployment:**
  - The presence of `CNAME` suggests GitHub Pages is used for deployment. Ensure the custom domain is set in repository settings.
- **External Dependencies:**
  - Bootstrap and Bootstrap Icons are loaded via CDN in each HTML file. No local or npm dependencies.

## Project-Specific Notes
- **Accessibility:**
  - ARIA attributes are present on navigation toggles for accessibility.
- **Color Scheme:**
  - The `<meta name="color-scheme" content="dark light">` tag and CSS media queries enable dark/light mode support.
- **No JavaScript Customization:**
  - Only Bootstrap's JS bundle is included; there is no custom JavaScript in this project.

## Example: Adding a New Page
1. Copy the structure of an existing HTML file (e.g., `About.html`).
2. Update the navigation bar and footer as needed.
3. Add your content within the `<main>` or main content section.
4. Reference any new images or assets directly by filename.

## Key Files
- `index.html`, `About.html`, `Contact.html`: Main site pages
- `style.css`: Custom styles for layout, color scheme, and responsiveness
- `CNAME`: Custom domain for GitHub Pages

---
For any global UI changes, update all HTML files for consistency. No build or test automation is present; all changes are manual and static.

# Website Documentation

## 1. Project Overview
This is a static personal portfolio website for a Solutions Architect profile.

It is focused on:
- AWS Solutions Architecture
- Terraform Provisioning
- PowerShell Automation
- GitHub and Git workflow setup
- AWS CLI usage

The visual direction is a black "midnight city" theme with cloud-technology accents.

## 2. Tech Stack
- HTML5 (`index.html`)
- CSS3 (`style.css`)
- Google Fonts (`Jost`)

No JavaScript framework or build tooling is required.

## 3. File Structure
- `index.html`: Page content and semantic layout (navigation, hero, services, about, contact, footer).
- `style.css`: Theme, layout, typography, responsive behavior, visual effects.
- `DOCUMENTATION.md`: Project documentation (this file).

## 4. Main Sections
- Navigation: Quick links to Services, About, Contact.
- Hero: Personal positioning and key value proposition.
- Services: Core services offered.
- About: Experience summary and tools/platform focus.
- Contact: Contact methods and inquiry form UI.
- Footer: Branding and hosting note.

## 5. Theme and Design Notes
- Base color is black (`--bg: #000000`).
- Surface/card layers use near-black shades for depth.
- Accent color uses cloud-tech cyan tones.
- Navigation links and CTA are styled as consistent floating pill buttons.
- Hero includes subtle atmospheric effects to suggest a midnight city/cloud look.

## 6. Typography
- Font family: `Jost` (sans-serif).
- Defined in:
  - `index.html` via Google Fonts link
  - `style.css` variables:
    - `--font-head`
    - `--font-mono`

## 7. Content Focus
Current positioning emphasizes:
- 1 year experience as a vibrant Solutions Architect
- AWS as the primary cloud platform
- Sustainable and cost-efficient solution design
- AI integration for better outcomes
- Tool stack: Terraform, PowerShell, GitHub, Git, AWS CLI

## 8. Local Preview
Open `index.html` directly in a browser.

Optional:
- Use a local static server for testing relative paths and caching behavior.

## 9. Deployment (AWS S3 Static Hosting)
1. Create an S3 bucket (same name as desired site domain if using custom domain).
2. Upload `index.html` and `style.css`.
3. Enable static website hosting in bucket properties.
4. Set index document to `index.html`.
5. Configure bucket policy/public access according to your security approach.
6. (Optional) Place CloudFront in front of S3 for HTTPS and CDN performance.

## 10. Maintenance Checklist
- Keep service descriptions aligned with your real offerings.
- Update experience summary over time.
- Verify all links (email, LinkedIn, GitHub).
- Test responsive layout after content changes.
- Version updates with Git before major edits.


# Solutions Architect Portfolio Website
[![Deploy static site to GitHub Pages](https://github.com/MastareeColnel/solutions-architect-web-app/actions/workflows/pages.yml/badge.svg)](https://github.com/MastareeColnel/solutions-architect-web-app/actions/workflows/pages.yml)

A static portfolio website focused on AWS Solutions Architecture, Terraform provisioning, PowerShell automation, and GitHub/Git workflows.

## Live Site
- https://mastareecolnel.github.io/solutions-architect-web-app/

## Live Theme
- Visual style: black "midnight city" with cloud-technology accents
- Typography: Jost (sans-serif)
- Layout: responsive single-page portfolio

## Tech Stack
- HTML5
- CSS3
- Google Fonts

## Project Structure
```text
.
|-- index.html
|-- style.css
|-- DOCUMENTATION.md
`-- README.md
```

## Sections
- Navigation
- Hero
- Services
- About
- Contact
- Footer

## Local Run
No build step is required.

1. Clone the repository
2. Open `index.html` in your browser

Optional: run with a local static server.

## Customize Content
Edit `index.html` for:
- personal description
- services
- tools/platform details
- links (email, LinkedIn, GitHub)

Edit `style.css` for:
- colors (`:root` variables)
- typography
- spacing/layout
- button and card styling

## Deploy to AWS S3 (Static Hosting)
1. Create an S3 bucket
2. Upload `index.html` and `style.css`
3. Enable Static Website Hosting
4. Set index document to `index.html`
5. Configure public access policy as needed
6. (Optional) Use CloudFront for HTTPS + CDN

## Deployment via AWS CLI (Example)
```bash
aws s3 sync . s3://your-bucket-name --exclude ".git/*" --exclude ".github/*"
```

## GitHub Push
```bash
git init
git add .
git commit -m "Initial portfolio website"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

## CI/CD
Yes. This repo now has a GitHub Actions pipeline that deploys to GitHub Pages on each push to `main`.
- CI part: workflow trigger and execution in GitHub Actions
- CD part: automatic deployment to GitHub Pages

## Notes
- Keep `DOCUMENTATION.md` for detailed project documentation.
- Update service offerings and About text as your profile evolves.

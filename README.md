# Personal Portfolio Website — Cloud Deployment Project

A responsive personal portfolio for **Mamunur Islam**, built with **HTML, CSS, and JavaScript** and designed to be hosted on **GitHub Pages**. This project demonstrates deployment of a static website to a publicly accessible cloud-hosted platform using a GitHub repository.

> **Deployment status:** The source code is ready for deployment. A live URL has not been configured or verified yet.

## Project overview

**Project title:** Personal Portfolio Website Deployment Using GitHub Pages  
**Project type:** Static website / cloud deployment  
**Hosting platform:** GitHub Pages  
**Technologies:** HTML5, CSS3, JavaScript  
**Author:** Mamunur Islam

### Objective

Develop a responsive personal portfolio and publish it on GitHub Pages to demonstrate basic cloud hosting, version control, and automated deployment from a Git repository.

## Features

- Responsive dark-themed design for desktop and mobile screens
- Sections for About, Skills, Projects, Experience, Research, Certifications, and Contact
- Mobile navigation menu
- Smooth section navigation and scroll-reveal effects (with reduced-motion support)
- Email and telephone contact links
- Single-file static site: no backend, database, or build step required

## Project structure

```text
portfolio/
├── index.html   # HTML structure, embedded CSS, and JavaScript
└── README.md    # Project documentation and deployment instructions
```

The website's CSS and JavaScript are embedded in `index.html`; separate `style.css` and `script.js` files are **not** required.

## Run locally

1. Download or clone the repository.
2. Open `index.html` in a web browser.
3. Check the navigation, sections, and mobile layout.

No dependencies or installation are needed. The site loads Google Fonts from a third-party CDN, so custom fonts may require an internet connection.

## Deploy to GitHub Pages (step by step)

1. Sign in to [GitHub](https://github.com).
2. Select **New repository** and name it `portfolio` (or another name).
3. Make the repository **Public** for the simplest GitHub Pages setup.
4. Upload `index.html` and `README.md` to the **repository root** and commit the files.
5. Open the repository's **Settings → Pages**.
6. Under **Build and deployment**, select **Deploy from a branch**.
7. Choose branch **main**, folder **/(root)**, then click **Save**.
8. Wait for the Pages deployment to complete. Check the **Actions** tab if it fails.
9. Return to **Settings → Pages** and open the published site link.

For a repository named `portfolio`, the expected project-site URL format is:

```text
https://YOUR_GITHUB_USERNAME.github.io/portfolio/
```

Replace `YOUR_GITHUB_USERNAME` with your actual username. This is an example URL, not a verified live deployment.

### Optional: Deploy using Git commands

If you already have an empty GitHub repository, from this folder run:

```bash
git init
git add index.html README.md
git commit -m "Initial portfolio website"
git branch -M main
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/portfolio.git
git push -u origin main
```

Then enable GitHub Pages in **Settings → Pages** as described above. If your repository already has commits or a configured remote, adapt these commands rather than blindly reinitializing it.

## Cloud deployment workflow

```text
Local website files
        |
        v
GitHub repository (main branch)
        |
        v
GitHub Pages build and deployment
        |
        v
Public HTTPS portfolio URL
        |
        v
Visitors on desktop and mobile browsers
```

**Deployment model:** GitHub Pages serves the static files over HTTPS. Committing and pushing changes to the selected branch triggers a new deployment. No application server or database is used.

## Testing checklist

- [ ] `index.html` opens correctly locally
- [ ] All navigation links scroll to the expected sections
- [ ] Mobile menu opens and closes
- [ ] Layout works on mobile and desktop
- [ ] Contact links behave as expected
- [ ] GitHub Pages deployment succeeds
- [ ] Public URL opens over HTTPS
- [ ] Updates pushed to `main` appear on the live website

## Common deployment issues

| Issue | Suggested fix |
| --- | --- |
| 404 page | Confirm `index.html` is in the repository root and Pages points to `main` / `/(root)`. |
| Site not live yet | Wait a few minutes and check the Actions deployment log. |
| Missing styles | Ensure the complete `index.html` was uploaded. |
| Changes not visible | Check deployment status and refresh the browser. |
| Broken external links | Replace placeholders with actual verified GitHub, LinkedIn, and project URLs. |

## Scope and limitations

- This is a **static** portfolio, not a full-stack application.
- GitHub Pages does not run a Python/Node.js backend or host a database for this site.
- The contact section uses `mailto:` and `tel:` links; it does not submit or store form data.
- GitHub, LinkedIn, and individual project repository URLs were not provided in the resume, so they are not represented as working links in this version.
- Do not put API keys, passwords, or other secrets in a public repository.

## Future enhancements

- Add verified GitHub, LinkedIn, and project repository links
- Add a downloadable resume PDF if you want it publicly accessible
- Add a custom domain
- Add automated link checking and accessibility tests through GitHub Actions

## References

- [GitHub Pages Quickstart](https://docs.github.com/en/pages/quickstart)
- [Configuring a publishing source for GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## License

No open-source license has been selected. Add a `LICENSE` file if you want to grant reuse rights.

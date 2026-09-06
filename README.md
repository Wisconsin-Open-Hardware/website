# Wisconsin Open Hardware (WOH) Website

This repository contains the source code for the Wisconsin Open Hardware (WOH) static website.

## Tech Stack
The site is built using pure, vanilla web technologies to remain lightweight, accessible, and easily maintainable by future generations of students without relying on complex build steps or node modules.
- HTML5
- CSS3 (Vanilla, custom properties for theming)
- JavaScript (Vanilla, for lightweight DOM interactions)

## Local Development
To run this site locally, you don't need any build tools. Simply clone the repository and open `index.html` in your browser.

Alternatively, you can serve it via a simple local HTTP server. E.g., using Python:
```bash
python3 -m http.server 8000
```
Then visit `http://localhost:8000` in your web browser.

## Deployment via GitHub Pages

This site is designed to be hosted directly on GitHub Pages. 

### To enable GitHub Pages:
1. Go to your repository settings on GitHub.
2. Navigate to **Pages** in the left sidebar.
3. Under **Source**, select `Deploy from a branch`.
4. Under **Branch**, select the `main` branch and the `/ (root)` folder.
5. Click **Save**.
6. GitHub will automatically build and deploy the site. It may take a few minutes for the initial deployment to complete.

### Setting up a Custom Domain
The club owns the domain name. Once the domain's DNS settings are configured to point to GitHub Pages, you can add it to the repo:
1. Go to the repository **Settings** -> **Pages**.
2. Under **Custom domain**, type the registered domain name and click **Save**.
3. This action will automatically commit a `CNAME` file to the root of the repository containing the domain name. 
4. **Ensure HTTPS is checked** to provide a secure connection for visitors.

## Updating Content (Placeholders)
There are several placeholders embedded in the HTML file (`index.html`) marked with `<!-- PLACEHOLDER: ... -->`. These need to be updated as real assets and information become available:
- **Logo**: Replace `assets/img/logo-placeholder.svg` with the actual SVG logo.
- **Email/Contact Links**: Update `mailto:placeholder@example.com` links.
- **GitHub Links**: Update `https://github.com/wisconsin-open-hardware` if the organization URL changes.
- **Leadership Photos**: Update the placeholder circles in the Leadership section with actual `<img>` tags if desired.
- **Faculty Advisor**: Update the text in the footer.
- **Governance**: Update the governance URL to point to the actual repo or document.

# CycleOne

## About the Project
A cutting-edge, performance-optimized website for Cycleone, delivering a seamless user experience with fluid animations and intuitive interactions across all devices.

## Live Website
**👉 [Live Website](https://cycleone.tech/)**

## Features
- **Fully Responsive Layout**: Adapts effortlessly to all screen sizes and devices
- **Optimized Performance**: Fast loading times with efficient animations
- **Interactive Elements**:
  - Smooth, animated team carousel with touch support
  - Intuitive navigation with scroll-spy functionality
- **Modern UI/UX**:
  - Clean, minimalist design
  - Subtle animations and transitions
  - Mobile-first approach

## Tech Stack
- **Frontend**: Semantic HTML5, CSS3 with Custom Properties for theming, Vanilla JavaScript (ES6+)
- **Animations**: The project uses [AOS](https://michalsnik.github.io/aos/) for scroll animations. AOS is loaded through a CDN in the HTML files. If animations stop working, check that the AOS CSS and JavaScript resources are loading correctly.

## Project Structure
```text
cycleone/
│
├── index.html              # Main landing page
├── about.html              # About us page
├── privacy-policy.html     # Privacy policy page
├── terms-of-service.html   # Terms of service page
├── style.css               # Main stylesheet
├── script.js               # Main JavaScript file
├── css/                    # Additional stylesheets
├── js/                     # Additional JavaScript files
├── components/             # Reusable HTML/UI sections
├── fonts/                  # Custom web fonts
├── images/                 # Image assets
└── CNAME                   # Custom domain configuration
```

## Local Development
1. **Clone the repository**
   ```bash
   git clone https://github.com/nareshshri23/Cycleone.git
   cd Cycleone
   ```
2. **Launch the application locally**
   You can simply open `index.html` in your browser, but using a local server is recommended to prevent asset loading issues.

   **Using Python (Recommended):**
   ```bash
   python -m http.server 8000
   # Open http://localhost:8000 in your browser
   ```

   **Using Node.js:**
   ```bash
   npx serve
   # Open http://localhost:3000 in your browser
   ```

   **Using VS Code:**
   - Install the **Live Server** extension and click "Go Live" at the bottom right.

## Git Workflow
We use a feature-branch workflow to keep the `main` branch stable.

### Before Starting New Work
Always update your local `main` before creating a new branch:
```bash
git checkout main
git pull origin main
```

### Workflow
1. **Create a branch**:
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b bugfix/issue-description
   ```
2. **Make and test your changes locally**.
3. **Commit your changes**:
   ```bash
   git add .
   git commit -m "Add new feature"
   ```
4. **Push your branch**:
   ```bash
   git push origin feature/your-feature-name
   ```
5. **Open a Pull Request** (PR) from your branch to `main`.
6. **Ask another contributor to review** the changes.
7. **Merge the PR** after approval.
8. **Delete the feature branch** after it has been merged.

### Rules
- Do **not** push directly to `main`.
- Create a separate branch for every feature or bug fix.
- Test your changes locally before creating a Pull Request.
- Create a Pull Request from your branch to `main`.
- Another contributor should review the Pull Request before merging.
- Delete the feature branch after the Pull Request is merged.
- Keep commit messages meaningful.
- Do not commit passwords, API keys, or other secrets.

## Deployment
The website is hosted using GitHub Pages.

- **Production URL:** https://cycleone.tech/
- **Hosting:** GitHub Pages
- **Deployment branch:** `main`
- **Custom domain:** `cycleone.in`
- **Custom domain configuration:** Managed through the `CNAME` file and DNS records

Any changes merged into `main` are deployed through GitHub Pages.

## Domain & DNS
- **Domain:** `cycleone.in`
- **Website hosting:** GitHub Pages
- **Custom domain:** Configured through GitHub Pages
- **DNS provider/registrar:** [Please verify: Namecheap / Cloudflare / other]

The `CNAME` file contains the custom domain configuration for GitHub Pages.
> **Note**: Do not store domain account passwords, API keys, or other credentials in this repository.

## Making Changes
- **Styling**: Update `style.css` or files within the `css/` directory. We use CSS Custom Properties (variables) for theming.
- **Functionality**: Update `script.js` or files within the `js/` directory. Ensure any new interactive elements are responsive.
- **Content**: Update the respective HTML files (`index.html`, `about.html`, etc.).
- **Components**: The `components/` directory contains reusable HTML snippets. If adding new reusable sections, ensure they are properly documented and integrated into the main HTML files.

## Testing
Before creating a Pull Request, test the website on:
- Desktop and mobile screen sizes
- Chrome, Edge, and Firefox (if possible)
- Navigation links
- Images and assets
- Light/dark mode
- Animations
- Responsive layout

## Environment Variables
This project is a static frontend website and does not require any environment variables for local development or deployment.

## Troubleshooting
- **Images not loading**: Verify the image paths in the HTML/CSS and ensure the images are placed correctly in the `images/` directory.
- **Animations not working**: Ensure the AOS library script is loading correctly.
- **Styles not applying**: Hard refresh the browser (Ctrl+F5 or Cmd+Shift+R) to clear the cache, or use a local dev server with hot reloading.

## Maintenance & Handover
CycleOne is a student-maintained project.

Future maintainers are responsible for:
- Website content and UI updates
- Bug fixes
- Responsive design improvements
- GitHub repository maintenance
- Deployment monitoring
- Domain/DNS configuration

Before making major changes, create an Issue describing the proposed change and discuss it with the current maintainers.

## Contributors
CycleOne is maintained by students and contributors from SLIET.

Contributors should follow the Git workflow described above when making changes.
- Naresh — Initial website development
- [Add Junior Names here]

## Contact
For inquiries or support, please contact [support@cycleone.in](mailto:support@cycleone.in)

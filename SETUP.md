# GitHub Profile README — Setup Guide

This package updates the existing GitHub profile repository for **Rafi7078**.

- Profile: https://github.com/Rafi7078
- Special profile repository: https://github.com/Rafi7078/Rafi7078
- Portfolio: https://salman-rafi-website.vercel.app/

## What is included

- `README.md` — redesigned profile page using the supplied midnight-navy and cyan visual system.
- `assets/` — the supplied visual assets are preserved. The README uses the newer `hero-reference.png`, the `nav-*-v6.png` buttons, and the matching section/project SVGs. The active `about.svg` replaces a conflicting location label with your professional focus areas.
- `SETUP.md` — this installation guide.

## Update the existing profile repository

The GitHub profile repository must be public and named exactly `Rafi7078` to display its README on `github.com/Rafi7078`.

### 1. Clone your existing profile repository

Open PowerShell in the folder where you keep your Git projects:

```powershell
git clone https://github.com/Rafi7078/Rafi7078.git
cd Rafi7078
```

If you already have this repository locally, open that folder instead. Do not create a second repository.

### 2. Back up the current README

```powershell
Copy-Item README.md README.backup.md
```

### 3. Copy the updated files

Extract this package. Copy these items from the extracted folder into your cloned `Rafi7078` repository:

- Replace `README.md`.
- Replace `SETUP.md`.
- Copy the complete `assets` folder, merging/replacing the existing assets folder.

Keep the `assets` folder beside `README.md` at the repository root.

### 4. Review the links

The active About graphic omits a location because the supplied GitHub profile screenshot and original About graphic showed different locations. This avoids publishing a conflicting location; add one back after confirming which location you want displayed.

The updated README points to:

- Portfolio: `https://salman-rafi-website.vercel.app/`
- LinkedIn: `https://www.linkedin.com/in/salmanrafi002/`
- GitHub: `https://github.com/Rafi7078`
- Email: `sajidbin7777@gmail.com`

The VerifyREST visual currently links to your GitHub repositories page because an exact public repository URL for that project was not present in the supplied README. Replace that link with the direct repository URL if you want to feature a specific public repository.

### 5. Commit and push

```powershell
git status
git add README.md SETUP.md assets/
git commit -m "Refresh GitHub profile to match portfolio branding"
git push origin main
```

If your profile repository uses a different default branch, push that branch instead of `main`.

### 6. Verify the profile

Open `https://github.com/Rafi7078` and refresh the page.

Check that:

- The new navy/cyan portrait banner appears.
- All six navigation buttons load.
- About, proof, selected work, skills, activity, credentials and footer graphics render.
- Project cards open the intended repositories.
- Portfolio, LinkedIn and email links work.

## Important notes

- This package changes the profile README and setup guide; it does not change your portfolio website or its Vercel deployment.
- The old portfolio URL has been replaced in the README with `salman-rafi-website.vercel.app`.
- GitHub README files support Markdown and limited HTML, not custom JavaScript. The visual assets are images, so the website's GSAP/React interactions do not run inside GitHub.
- The typing line depends on the external `readme-typing-svg` service. If that service is temporarily unavailable, the rest of the profile still renders.
- The contribution panel is a designed visual. Use the linked GitHub profile page to see your authentic, live contribution activity.
- No follower counts, stars, awards, or other changing statistics have been invented.

## Updating the GitHub profile website field

The website shown in the left sidebar of your GitHub profile is separate from this README.

1. Open `https://github.com/settings/profile`.
2. Find the **Public profile** section.
3. Set the **Website** field to `https://salman-rafi-website.vercel.app/`.
4. Save the changes.

This updates the sidebar website link without changing your other Vercel project.

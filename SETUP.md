# Premium GitHub Profile — Setup Guide

This package replaces the content of your **existing** GitHub profile repository:

https://github.com/Rafi7078/Rafi7078

## Files to upload

- `README.md` — GitHub profile content.
- `assets/header.svg` — custom profile hero.
- `assets/peoplemind.svg`, `assets/verifyrest.svg`, `assets/playwright.svg`, `assets/brain-tumor.svg` — project visuals.

## Fastest setup on Windows (PowerShell)

1. Back up your current profile `README.md` (optional but recommended).
2. Open PowerShell in your preferred work folder and run:

```powershell
git clone https://github.com/Rafi7078/Rafi7078.git
cd Rafi7078
```

3. Extract the ZIP file. Copy the supplied `README.md` and entire `assets` folder into your cloned `Rafi7078` folder. Choose **Replace** if Windows asks to overwrite `README.md`.
4. Review the contact details and link targets in the README.
5. Run:

```powershell
git add README.md assets/
git commit -m "Upgrade GitHub profile portfolio"
git push origin main
```

6. Visit https://github.com/Rafi7078 and refresh the page.

If the default branch is not `main`, push the actual default branch instead.

## A few intentional choices

- Uses **your existing public repositories**; it does not claim unverified live deployments.
- Uses custom local SVG graphics so the main banner and project illustrations do **not** depend on third-party image sites.
- Social badges, the animated line, and the optional GitHub stats use external services and need an internet connection.
- The GitHub stats are **collapsed by default** to keep the profile clean and reduce the impact of third-party outages.
- No phone number, home address, false awards, inflated rating, or misleading health-related performance claims are included.
- Markdown and HTML render inside the GitHub profile README; JavaScript does not run there.

## Optional customization

- Colors are specified directly in `assets/*.svg` files. The palette is midnight navy, electric cyan, teal, and lilac.
- Replace the title line `QA Automation / Applied AI / Data Analytics` in `assets/header.svg` if you change your career focus.
- Update your social links and email in `README.md` when needed.
- To feature different projects, update both the project table links and their captions.
- Re-pin relevant projects in GitHub Profile > Customize your pins. This is separate from the README.

## Troubleshooting

- **Images missing:** Confirm the SVGs were uploaded into the repo's exact `assets/` folder, beside README.md.
- **Profile does not update:** Confirm the repository is public, named exactly like the username (`Rafi7078`), and README.md is in its root and on its default branch.
- **External badges unavailable:** They are provided by shields.io or readme-typing-svg and may temporarily fail; the banner and project assets remain local.

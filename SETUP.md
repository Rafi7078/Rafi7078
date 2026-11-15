# GitHub Profile — Portfolio-Matched Edition

This package redesigns the profile README for **Rafi7078** to follow the visual identity of the portfolio website:

- Portfolio: https://salman-rafi-website.vercel.app/
- Profile: https://github.com/Rafi7078
- Special profile repository: https://github.com/Rafi7078/Rafi7078

## Visual direction

The previous README used a futuristic navy/cyan dashboard style. This edition intentionally replaces that direction with the portfolio's actual visual language:

- near-black and warm cream backgrounds
- restrained yellow accents
- oversized editorial typography
- small monospaced section labels
- numbered sections from 01 to 07
- simple text navigation and project links
- the portfolio portrait in the hero banner
- no neon buttons, stats cards, typing animation, or cyberpunk graphics

## Package contents

- `README.md` — complete replacement for the GitHub profile README.
- `assets/portfolio-hero.png` — new hero banner.
- `assets/section-01.svg` through `assets/section-07.svg` — matching section title graphics.

## Install on Windows

Use the cloned profile repository, not the portfolio website repository.

Expected local repository:

```powershell
C:\Users\RAFI\Downloads\Rafi7078-live
```

Copy the new `README.md` and `SETUP.md` into that folder, replacing the previous versions. Merge the new `assets` folder into the existing `assets` folder. The new assets use unique names (`portfolio-hero.png` and `section-01.svg` through `section-07.svg`), so the previous files can remain in place; the new README no longer references the old navy/cyan graphics.

Then run:

```powershell
cd C:\Users\RAFI\Downloads\Rafi7078-live
git diff --check
git status
git add README.md SETUP.md assets/portfolio-hero.png assets/section-*.svg
git commit -m "Redesign GitHub profile to match portfolio"
git push origin main
```

If `git status` shows unrelated changes that you did not intend, stop and review them before committing.

## GitHub README limitations

GitHub profile READMEs support Markdown and a limited subset of HTML. They do not run the portfolio's React, GSAP, JavaScript, cursor interactions, scroll animations, or theme toggle. This package matches the portfolio's static visual identity while keeping navigation and repository links functional.

## Content accuracy

The experience, education, projects, tools and training listed in the README are based on the supplied CV/profile materials. Personal phone numbers and reference contact details are intentionally excluded.

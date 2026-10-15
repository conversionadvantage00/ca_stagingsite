# Conversion Advantage website: live preview

The working version of the new Conversion Advantage homepage, packaged to run on GitHub Pages so it can be checked on real phones and browsers.

This is a **preview**, not the live site. It is set to `noindex`, so Google won't list it.

## What's in here

```
index.html            the homepage (everything in one file)
assets/industries/    popular industries photos (webp)
assets/logos/         45 client logos for the brands marquee (webp)
assets/media/         social media card video (webm + mp4) and its poster image
assets/fonts/         coolvetica (the brand display font) as a web font
.nojekyll             tells GitHub Pages to serve the files exactly as they are
README.md             this file
```

The page loads GSAP 3.12.5, ScrollTrigger and Lenis 1.1.20 from public CDNs, and its stand-in fonts from Google Fonts (Figtree for body text; Bricolage Grotesque only as a backup if Coolvetica can't load). Everything else is in this folder.

## Put it online (about 5 minutes)

1. Sign in at [github.com](https://github.com) and click **New repository** (the **+** at the top right).
2. Name it, for example `ca-website-preview`. Choose **Public**, because GitHub Pages is free for public repositories. Don't add a README; this folder has one. Click **Create repository**.
3. On the next screen, click **uploading an existing file**.
4. Unzip this folder on your computer. Then drag **everything inside it** into the upload box: `index.html`, `README.md`, `.nojekyll` and the `assets` folder.
   - Mac hides files that start with a dot. Press **Cmd + Shift + .** in Finder to show `.nojekyll`.
   - Make sure `index.html` lands at the top level of the repository, not inside another folder.
5. Click **Commit changes**.
6. Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*, **Branch** to `main` and the folder to `/ (root)`. Click **Save**.
7. Wait a minute or two, then refresh that page. GitHub shows the address, for example:
   `https://YOUR-USERNAME.github.io/ca-website-preview/`

Open that link on your phone and desktop.

## Updating it

When Claude sends a new version, open the repository on GitHub, click **Add file → Upload files**, and drag in the changed files (usually `index.html`, and sometimes new files in `assets/`). Uploading a file with the same name replaces the old one. Click **Commit changes**; the live link updates within a minute or two.

If an update doesn't show, do a hard refresh: **Cmd + Shift + R** on Mac or **Ctrl + Shift + R** on Windows. On a phone, close the tab and open the link again.

## Good to know

- **Fonts:** Coolvetica is included, so every device shows the real display font. The body text still uses the stand-in (Figtree) until the Aspekta files are added.
- **Buttons:** "learn more", "find out how", "all success stories" and "see microsites" are not linked yet. Their pages don't exist yet.
- **This is a preview only.** The planned production setup is GitHub plus Cloudflare Pages, with media on Bunny.net. GitHub Pages is just a quick way to test the real thing on real devices.
- **Source of truth:** the master copy lives in Google Drive › My Drive › Claude Code › ca-website › working. This repository is a copy for viewing.

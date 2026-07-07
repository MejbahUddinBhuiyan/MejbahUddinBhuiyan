# Premium GitHub Profile Setup Guide

This repository is a complete premium GitHub Profile README system for **Mejbah Uddin Bhuiyan**.

## 1. Create your profile repository

Create a public repository with the exact same name as your GitHub username.

Example:

```text
MejbahUddinBhuiyan/MejbahUddinBhuiyan
```

GitHub will automatically display `README.md` on your profile page.

## 2. Upload the files

Upload this full structure:

```text
README.md
assets/
  banner.svg
  divider.svg
  gradient.svg
  footer.svg
  icons/
.github/workflows/
  snake.yml
  metrics.yml
docs/
  setup.md
```

## 3. Replace placeholders

Search the README for these placeholders and replace them:

```text
YOUR_LINKEDIN_USERNAME
YOUR_RESEARCHGATE_USERNAME
YOUR_FACEBOOK_USERNAME
YOUR_INSTAGRAM_USERNAME
YOUR_LEETCODE_USERNAME
YOUR_CODEFORCES_USERNAME
YOUR_HACKERRANK_USERNAME
YOUR_EMAIL@example.com
```

Also replace `MejbahUddinBhuiyan` if your actual GitHub username is different.

## 4. Add GitHub Metrics token

GitHub Metrics works best with a Personal Access Token.

Create a classic GitHub token with safe read permissions, then add it as a repository secret:

```text
Settings → Secrets and variables → Actions → New repository secret
Name: METRICS_TOKEN
Value: your_token_here
```

## 5. Enable workflows

Go to:

```text
Actions → Generate Contribution Snake → Run workflow
Actions → Generate GitHub Metrics → Run workflow
```

The workflows will generate files inside:

```text
assets/generated/
```

## 6. Profile picture

The banner currently contains a professional placeholder. For a real profile photo, either:

1. Edit `assets/banner.svg`, or
2. Add `assets/profile.png` and create a small image block in the README.

## 7. Recommended maintenance

- Keep project cards updated.
- Add real repository links after publishing projects.
- Add DOI or paper URL for the publication when available.
- Review third-party widgets every few months.
- Keep the README minimal, premium and stable.

## 8. Notes on external widgets

This profile intentionally avoids large badge collections and unstable image services.

Used dynamic services:

- GitHub Metrics via `lowlighter/metrics`
- Contribution Snake via `Platane/snk`
- Typing SVG via `DenverCoder1/readme-typing-svg`

Most visual identity is local SVG, so the profile remains elegant even if dynamic widgets are delayed.

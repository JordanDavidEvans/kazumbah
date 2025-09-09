# Kazumbah Hugo Site

This repository contains a minimal [Hugo](https://gohugo.io/) website designed to be deployed via a Cloudflare Worker or Pages project.

## Local development

1. Install the extended version of Hugo.
2. Build the site locally:

   ```bash
   hugo server
   ```

   The generated site is served from `http://localhost:1313`.

## Cloudflare deployment

When configuring the Cloudflare Worker/Pages project:

- **Build command:** `hugo`
- **Build output directory:** `public`
- **Environment variables:**
  - `HUGO_VERSION`: `0.123.7` (or your preferred version)
  - `NODE_VERSION`: `20` (needed for Hugo Pipes when using PostCSS/Sass)

These settings ensure Cloudflare installs the correct Hugo binary and outputs the generated site to the `public` directory.

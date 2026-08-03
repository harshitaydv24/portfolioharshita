# Harshita Yadav — Portfolio Website

A single-page portfolio built with plain HTML, CSS, and JavaScript — no build step, no dependencies, no framework. Everything (styles, scripts, and images) lives inside `index.html`, so it can be hosted anywhere that serves static files.

## Files in this folder

| File | Purpose |
|---|---|
| `index.html` | The entire website — HTML, CSS, JS, and all images (base64-embedded) |
| `robots.txt` | Tells search engines they're allowed to crawl the site |
| `sitemap.xml` | Helps search engines discover the page |
| `README.md` | This file |

## Option 1: Deploy with GitHub Pages (recommended, free)

You already have GitHub Pages projects live (`weather-app`, `tic-tac-toe`, etc.), so this will feel familiar.

1. Create a new repository on GitHub named exactly:
   ```
   harshitaydv24.github.io
   ```
   (This special name makes it your main profile site instead of a project page.)
2. Upload `index.html`, `robots.txt`, and `sitemap.xml` to the repo (drag-and-drop on GitHub, or via git):
   ```bash
   git init
   git add index.html robots.txt sitemap.xml
   git commit -m "Deploy portfolio"
   git branch -M main
   git remote add origin https://github.com/harshitaydv24/harshitaydv24.github.io.git
   git push -u origin main
   ```
3. Go to the repo's **Settings → Pages**, and under "Build and deployment," set Source to **Deploy from a branch**, branch **main**, folder **/(root)**.
4. Wait 1–2 minutes, then visit `https://harshitaydv24.github.io/` — it's live.

## Option 2: Deploy with Netlify (also free, drag-and-drop)

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the whole folder (or just `index.html`) onto the page
3. Netlify gives you a live URL immediately — you can rename it or connect a custom domain in site settings

## Option 3: Deploy with Vercel

1. Go to [vercel.com/new](https://vercel.com/new)
2. Import the folder as a new project (no framework preset needed — choose "Other")
3. Deploy — Vercel gives you a live URL instantly

## After deploying: update your Web3Forms URL

The contact form uses [Web3Forms](https://web3forms.com) to send messages to your inbox. Once your site has a real live URL:

1. Log in to your Web3Forms dashboard
2. Update the **Website URL** on your form from `localhost` (or whatever you entered) to your real deployed URL (e.g. `https://harshitaydv24.github.io`)
3. Test the form on the live site to confirm the email arrives

## Making future edits

Since everything is in one file, editing is simple:
- Open `index.html` in any text editor (VS Code, etc.)
- All CSS is inside the `<style>` tag near the top
- All JavaScript is inside the `<script>` tag near the bottom
- Re-upload/redeploy the file after any change (GitHub Pages, Netlify, and Vercel all auto-redeploy on new commits/uploads)

## Custom domain (optional)

All three hosting options above support connecting a custom domain (e.g. `harshitayadav.com`) for free if you own one — look for "Custom domain" in your host's settings once deployed.

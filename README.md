# Vaishnavi Jagtap — Portfolio

A single-page portfolio site, rebuilt from the original Google Sites portfolio
(sites.google.com/view/vaishnavij-portfolio), ready to host on GitHub Pages.

## What's here

- `index.html` — all content: home, about, experience, education, skills,
  featured project, more work, other work, and contact
- `styles.css` — site styling
- `script.js` — mobile nav toggle + active-section highlighting
- `images/` — all site images, self-hosted (no more hotlinking to Google's CDN)
- `Vaishnavi_Jagtap_CV_Data_Engineer.pdf` — the CV linked from the About section

## About the invitation card image

`images/canva-invitation-card.jpg` is a cropped version of the Vastu Shanti
invitation you designed. The venue address and both phone numbers from the
bottom of the original card have been cropped out before publishing, since
that's not something to have sitting on a public site. If you'd rather leave
the whole card out entirely, just remove that `<figure>` block from the
"Canva design" section in `index.html`.

## Publish it on GitHub Pages (no command line needed)

1. Go to [github.com/new](https://github.com/new) and create a repository
   named exactly **`vaimeraki.github.io`** (matching your GitHub username
   this way gives you a live site at `https://vaimeraki.github.io`
   automatically). Leave it public, and don't initialize it with a README.
2. On the new repo's page, click **"uploading an existing file"**.
3. Drag in `index.html`, `styles.css`, `script.js`,
   `Vaishnavi_Jagtap_CV_Data_Engineer.pdf`, and the whole `images` folder
   from this project, then click **Commit changes**.
4. Go to **Settings → Pages** in the repo. Under "Build and deployment",
   set Source to **Deploy from a branch**, branch **main**, folder **/(root)**,
   then **Save**.
5. Give it a minute, then visit `https://vaimeraki.github.io` — your site
   should be live.

If you'd rather use `git` from the command line instead of the upload
button, the flow is:

```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/vaimeraki/vaimeraki.github.io.git
git push -u origin main
```

# Personal Website

## File structure

```
personal-site/
├── index.html              ← Homepage
├── css/
│   └── style.css           ← All shared styles — edit colours/fonts here
├── pages/
│   ├── education.html
│   ├── research.html
│   ├── publications.html
│   ├── dance.html
│   └── contact.html
├── files/
│   └── cv.pdf              ← Put your CV here
└── images/
    └── photo.jpg           ← Put your headshot here
```

## How to customise

1. **Your name and role** — search for "Your Name" across all files and replace.
   Every page has it in the sidebar and page title.

2. **Profile photo** — add your photo as `images/photo.jpg`, then in `index.html`
   replace the placeholder div with:
   ```html
   <img src="images/photo.jpg" alt="Your Name">
   ```

3. **CV** — put your CV PDF in `files/cv.pdf`. All "Download CV" links already
   point there.

4. **Colours** — open `css/style.css` and edit the `:root` block at the top:
   - `--accent` is the teal green used for links and highlights
   - `--ink` is the main text colour
   - `--bg` is the page background

5. **Navigation active state** — on each page, the current page's `<a>` tag has
   `class="active"`. This is already set correctly on every page.

6. **Add a page** — copy any existing page file, update the `<title>`, the
   sidebar active class, and the content. Then add a link in the sidebar of
   every other page.

## How to publish (free options)

### GitHub Pages (recommended — free, fast, custom domain)
1. Create a GitHub account if you don't have one
2. New repository → name it `yourusername.github.io`
3. Upload all files (maintaining the folder structure)
4. Go to Settings → Pages → Source: main branch → Save
5. Your site is live at `https://yourusername.github.io`

### Netlify (also free, easier drag-and-drop)
1. Go to netlify.com → sign up
2. Drag your `personal-site/` folder onto the deploy area
3. Done — you get a URL like `yourname.netlify.app`
4. You can connect a custom domain (e.g. yourname.com) for ~£10/year

### Custom domain
Buy `yourname.com` from Namecheap or Cloudflare (~£10/year), then point
it at your GitHub Pages or Netlify deployment. Both have simple guides.

## Maintenance tips

- To add a publication: copy one `<div class="pub-entry">` block in
  `publications.html` and fill in the details. No coding needed.
- To add a news item: copy one `<div class="news-item">` block in `index.html`.
- To add a performance: copy one `<div class="perf-entry">` block in `dance.html`.
- Update "Last updated" in the sidebar footer of each page when you make changes.

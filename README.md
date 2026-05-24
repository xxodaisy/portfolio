# Personal Portfolio — Your Name

A minimal, fast, and recruiter-friendly portfolio site built with plain HTML/CSS/JS. No frameworks, no build tools — just one file.

**Live site:** [yourname.vercel.app](https://yourname.vercel.app)

---

## Features

- Dark / light mode with system preference detection
- Downloadable CV
- Project cards with visual thumbnails
- Blog section linking to Medium
- Bold contact closer
- Fully responsive (mobile + desktop)

## Stack

- Plain HTML, CSS, JS — zero dependencies
- Hosted on [Vercel](https://vercel.com)
- Fonts via Google Fonts (Lora + DM Sans)

## Structure

```
portfolio/
├── index.html        # entire site lives here
└── cv-yourname.pdf   # your CV — rename as needed
```

Optional: add an `/images` folder for real project/blog screenshots.

```
portfolio/
├── index.html
├── cv-yourname.pdf
└── images/
    ├── project1.png
    ├── project2.png
    ├── project3.png
    ├── blog1.png
    ├── blog2.png
    └── blog3.png
```

## Customization

All content lives in `index.html`. Find and replace the following:

| Placeholder | Replace with |
|---|---|
| `Your Name` | Your full name |
| `your@email.com` | Your email |
| `yourname` (in all links) | Your handle |
| `cv-yourname.pdf` | Your actual CV filename |
| Project titles, descriptions, tools | Your real projects |
| Blog titles, dates, links | Your actual posts |

To swap placeholder thumbnails for real screenshots, replace the `<div class="project-thumb">` blocks in each project card with:

```html
<img src="/images/project1.png" alt="Project name"
     style="width:100%;height:160px;object-fit:cover;display:block;">
```

Same pattern for blog thumbnails — replace `<div class="blog-thumb">` with a 80×60 `<img>`.

## Local Preview

No build step needed. Just open the file:

```bash
open index.html
# or drag it into any browser
```

For a local server (optional):

```bash
npx serve .
```

## Deployment

Deployed via Vercel connected to this GitHub repo. Every push to `main` triggers an automatic redeploy.

---

Made with plain HTML · Deployed on Vercel

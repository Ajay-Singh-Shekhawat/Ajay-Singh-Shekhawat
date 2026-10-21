# Project context

This repository contains Ajay Singh Shekhawat's personal portfolio website.
User experience is the top priority: keep the site intuitive, readable,
accessible, and polished across browsers on desktop, Android, and iOS. Keep
the design professional, concise, and responsive. The homepage and contact
page should fit on a typical screen without scrolling; the resume page may
scroll.

Do not publish or reintroduce Ajay's phone number. Public contact details are
his email address and LinkedIn profile. Keep resume claims aligned with the
resume content supplied by Ajay; do not reintroduce the incorrect claim about
a Cassandra library being used in 19 repositories. His experience summary is
8.5+ years.

# Project structure

- `public/index.html`: concise homepage.
- `public/resume.html`: recruiter-friendly, scannable resume.
- `public/contact.html`: email and LinkedIn contact page.
- `public/styles.css`: shared responsive styles and print styles.
- `public/script.js`: small shared navigation and footer behavior.
- `public/Ajay-Singh-Shekhawat-Resume.pdf`: manually maintained downloadable
  resume PDF.
- `server.js`: dependency-free local preview server; it is not required to
  host the static site.

# Development and deployment

- Requires Node.js 18 or newer. No npm dependencies are required.
- Run `npm start` to preview the site locally (defaults to port 3000; set
  `PORT` to use another port).
- The resume PDF is a static file. Replace it manually in `public/` when
  updating the downloadable resume.
- Cloudflare Pages can deploy the static site directly from GitHub with
  `public` as the output directory and no build command. The Node preview
  server is not the Cloudflare Pages runtime.

# Change guidelines

- Prioritize user experience in every change: use semantic HTML, responsive
  layouts, accessible navigation and focus states, touch-friendly controls,
  and interactions that work with mouse, keyboard, and touch. Keep all pages
  usable without a framework or client-side routing.
- Keep page content and the manually maintained downloadable PDF consistent
  when changing resume facts. Never add personal contact details beyond the
  published email and LinkedIn without Ajay's explicit request.
- Avoid adding dependencies unless a requirement cannot reasonably be met
  with the existing Node.js and browser APIs.

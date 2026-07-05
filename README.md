# Monika Gopinathan — Portfolio

A five-page static portfolio site: Home, Experience, Skills, Projects, Contact.
Plain HTML/CSS/JS — no build step, no framework, works anywhere.

## Structure

```
.
├── index.html          Home — hero, summary, capabilities, previews
├── experience.html      Career timeline + education
├── skills.html           Full skill set by category
├── projects.html        Case studies (4 featured projects)
├── contact.html         Contact details + résumé download
├── css/style.css        All styling (one shared file)
├── js/main.js            Nav toggle, hero animation, copy-to-clipboard
├── assets/
│   ├── Monika_Gopinathan_Resume.pdf   ← your résumé, downloadable
│   └── favicon.svg
└── README.md
```

## Host it on GitHub Pages (free)

1. Create a new GitHub repository — e.g. `monika-portfolio`.
2. Upload every file in this folder to the repository, keeping the folder structure intact.
3. In the repo, go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
5. GitHub gives you a live URL within a minute or two, usually:
   `https://<your-username>.github.io/monika-portfolio/`

If you'd rather use a custom domain, add it in the same **Pages** settings screen — GitHub walks you through the DNS records.

### From your computer, with git

```bash
cd portfolio
git init
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin https://github.com/<your-username>/monika-portfolio.git
git push -u origin main
```

Then turn on Pages as described above.

## Before you publish — a few things to update

- **LinkedIn link** — `contact.html` has a placeholder `href="#"` on the LinkedIn card. Replace it with your real profile URL.
- **Résumé file** — swap `assets/Monika_Gopinathan_Resume.pdf` for a newer version any time; the filename can stay the same so the download links keep working.
- **"Open to new opportunities" banner** — in `contact.html`, remove or edit the `.status-banner` div once you're no longer looking.
- **Copyright year** — the footer says `© 2026`; update yearly, or replace with just your name.

## Editing content

Every page is a normal HTML file — open any of them in a text editor and edit the text directly. Shared look and feel lives in `css/style.css`, so a change there (e.g. the accent colour `--mint` at the top of the file) updates every page at once.

## Other free hosting options

The site is plain static files, so any of these work too, with no changes required:
- **Netlify** — drag the `portfolio` folder onto netlify.com/drop
- **Vercel** — `vercel deploy` from inside the folder
- **Cloudflare Pages** — connect the GitHub repo and deploy

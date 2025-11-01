FabricFashion — Static site

This folder contains a static website for "FabricFashion" (HTML, CSS, images).

Quick hosting options (free):

1) GitHub Pages (recommended if you use GitHub)
- Create a public GitHub repository and push this folder
- In PowerShell (from project root):
  git init ; git add . ; git commit -m "Initial site" ; git branch -M main
  # create repo on GitHub (web or `gh repo create`) and add remote, then:
  git remote add origin https://github.com/<your-username>/<repo>.git ; git push -u origin main
- Enable Pages in repository Settings -> Pages -> Source: main / (root)

2) Netlify (drag-and-drop or connect to GitHub)
- Go to https://app.netlify.com/, sign up and either drag-and-drop the project folder to Sites or connect to GitHub and choose the repo.
- Netlify auto-builds and provides a free TLS-enabled URL.

3) Cloudflare Pages
- Go to https://pages.cloudflare.com/, sign up and connect your GitHub repo.
- Configure the build to be a "Static site", but for plain HTML you can leave the build command blank and the root as '/'.

Custom domain and SSL
- All of the above support custom domains. Add a DNS A or CNAME record as directed by the provider.
- Providers automatically provision TLS (Let's Encrypt) for your domain in most cases.

If you'd like, I can:
- Create a GitHub repo and push the files (I will need your permission and a token), or
- Prepare a one-click Netlify deploy config, or
- Add a CNAME file if you already have a custom domain.

Notes
- I added a blank `.nojekyll` file to ensure GitHub Pages serves files starting with underscores or folders correctly.
- Open help.html in your browser to preview locally, or run: python -m http.server 8000

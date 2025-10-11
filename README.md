# Hydratech Industries — Static Site Starter

This folder contains a minimal, professional static website ready for **GitHub Pages** with a **custom domain**.

## Quick Start

1. Create a GitHub account (or organization) and sign in.
2. Create a new repository (e.g., `hydratech-site`).
3. Upload all files from this folder to the repository root.
4. Go to **Settings → Pages** in your repo:
   - **Build and deployment**: Source = `Deploy from a branch`
   - Branch = `main`, Folder = `/ (root)` → Save
5. (Optional) Commit the provided `CNAME` file to set your custom domain: `hydratechindustries.org`.
6. In your domain registrar (e.g., GoDaddy/Namecheap), set DNS records:

### DNS for apex/root domain (`hydratechindustries.org`)

Create **A** records pointing to GitHub Pages:

- A → 185.199.108.153
- A → 185.199.109.153
- A → 185.199.110.153
- A → 185.199.111.153

*(If your DNS supports ALIAS/ANAME for the root, you can use that instead of A records.)*

### DNS for `www.hydratechindustries.org` (optional)

Create a **CNAME** record:  
`www` → `<YOUR_GITHUB_USERNAME>.github.io`

> Replace `<YOUR_GITHUB_USERNAME>` with your actual GitHub username (or org name).

7. In **Settings → Pages**, enter your **Custom domain**: `hydratechindustries.org`, save, and **enforce HTTPS** once available.

## Editing Content

- Update text in `index.html` to match your brand (hero, About, Technology, etc.).
- Replace `assets/favicon.png` with your logo or icon (16–512px square).
- For a contact form, consider services like Formspree/Getform and swap the `mailto:` link.

## Notes

- The included `CNAME` file helps GitHub automatically keep your custom domain setting.
- Changes to DNS can take time to propagate. If you see a 404 at first, give it a bit and re-check HTTPS settings in Pages.

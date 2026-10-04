# Yopi website

Static website for the Yopi app: home page, Privacy Policy, Terms of Use, Contact and a 404 page.
No build step. Upload the files and it works.

## 1. Replace the placeholders (do this first)

Search all `.html` files and `sitemap.xml` / `robots.txt` for these and replace them:

| Find | Replace with |
|---|---|
| `support@yopi.app` | your real support email |
| `https://apps.apple.com/app/id0000000000` | your App Store link |
| `https://yopi.app` | your website address (for example `https://yourname.github.io/yopi-site`) |
| `© 2026 Yopi` | your company or developer name, if different |

In VS Code: Edit → Replace in Files (Cmd/Ctrl + Shift + H).

Also check the Privacy Policy section "Storage, retention and deletion" matches what your app really does (it says uploads are deleted within 30 days).

## 2. Host on GitHub Pages

1. Create a new **public** repository on github.com (for example `yopi-site`).
2. Click **Add file → Upload files** and drag in everything from this folder (including the `assets` folder and the `.nojekyll` file). Commit.
3. Go to **Settings → Pages**. Under "Build and deployment" choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After a minute your site is live at `https://YOUR-USERNAME.github.io/yopi-site/`.

Your links for App Store Connect:
- Privacy Policy URL: `https://YOUR-USERNAME.github.io/yopi-site/privacy.html`
- Support URL: `https://YOUR-USERNAME.github.io/yopi-site/contact.html`
- Marketing URL: `https://YOUR-USERNAME.github.io/yopi-site/`

## 3. Custom domain (optional)

In **Settings → Pages → Custom domain**, enter your domain (for example `yopi.app`) and follow GitHub's DNS instructions. Then tick **Enforce HTTPS**.

## Files

- `index.html`: home page
- `privacy.html`: Privacy Policy (includes face data section Apple asks for)
- `terms.html`: Terms of Use (subscriptions, auto-renewal, acceptable use)
- `contact.html`: contact form (opens the visitor's email app) and quick answers
- `404.html`, `robots.txt`, `sitemap.xml`, `.nojekyll`
- `assets/`: styles, icon, screenshots, app preview video

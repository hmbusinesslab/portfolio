# HM Business Lab — launch package

This is the current website, including your video, animation, portrait, and a Decap Turbo-backed Diary.

## 1. Publish on GitHub Pages

1. Create a GitHub repository named `portfolio`, with branch `main`.
2. Unzip this package and upload the CONTENTS of this folder to the repository root (not the containing folder or ZIP). Include `.github/workflows/pages.yml` and `.nojekyll`. If the browser uploader omits dotfolders, upload them with GitHub Desktop or create `.github/workflows/pages.yml` using Add file > Create new file and paste its contents.
3. Open repository Settings > Pages, and choose GitHub Actions as the source.
4. In Actions, open Publish website and run the workflow if needed. Wait for success. The deployment provides the website URL.

## 2. Connect your existing Decap Turbo account

1. In Turbo, create/select your organization and connect GitHub. Grant the Turbo GitHub App access only to this repository.
2. Create a Turbo site: repository hmbusinesslab/portfolio; branch main; config path admin/config.yml; admin URL https://hmbusinesslab.github.io/portfolio/admin/ (replace with the actual deployment URL).
3. Copy the Site ID from that site's Overview page. This is a public identifier, not a password or token.
4. Edit admin/config.yml in GitHub. Replace REPLACE_WITH_YOUR_TURBO_SITE_ID with that Site ID, then commit. The website redeploys automatically.
5. Open your deployed /admin/ URL and choose Login with Turbo.

Do not share passwords, private keys, or access tokens. CMS authentication is handled by Turbo; there is no password embedded in this website. Login cannot work until the real Site ID and allowed admin URL are configured.

## 3. Write articles

In the editor open The Business Diary > Articles. Add an item, set its title, unique lowercase-hyphen URL name, category, date, introduction, optional image, and article body. Enable Show on website to include it, then save/publish. Wait for GitHub Pages deployment, then refresh the public diary. Disable Show on website to remove an entry from the public list. Remove a list item to delete it.

The repository is the content source. In a PUBLIC repository, all committed content (including entries with Show on website off) is publicly readable. Do not store confidential drafts here. The public page's visibility setting is not access control.

The initial Diary is empty. Earlier sample drafts were intentionally excluded from the launch package. Markdown supports paragraphs, bold, italic, second/third-level headings, and bullet lists. Raw HTML is escaped. Choose a cover image through the dedicated image field.

## Contact delivery

The inquiry form now explicitly hands the visitor to WhatsApp at +30 694 845 2965. The visitor must press Send in WhatsApp. It does not claim an email was delivered. The final page provides an Open WhatsApp link if popup blocking prevents opening. A dedicated email/form service can be connected later.

## Domain

After the default GitHub Pages URL works, add your domain in repository Settings > Pages and configure the DNS records shown by GitHub. Enable HTTPS once the certificate is ready. Add the new /admin/ URL to Decap Turbo too. No domain has been configured in this package.

## Before announcing

Test the site on desktop and mobile, confirm the contact number, send a real WhatsApp inquiry, verify the social links, log into /admin/, publish a test post, and verify it appears after deployment. The site requires network access for Google Fonts and the Decap editor script.

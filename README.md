# Deals With Justin — personal link-in-bio website

A personal, mobile-friendly deal-sharing page with Justin's supplied profile picture, quick links, deal cards, Amazon/Walmart filters, price filters, search, promo codes, and a local editor.

## Publish the redesign to GitHub Pages

1. Unzip this package.
2. Open the GitHub repository you already use for your website.
3. Upload **the contents of this folder**, not the folder itself. Replace existing `index.html`, `styles.css`, `app.js`, `config.js`, `deals.json` and add `justin-profile.png`.
4. Commit changes. Check Settings → Pages to confirm deployment.
5. Hard-refresh the public site after GitHub finishes deploying.

The profile image must sit alongside `index.html` in the repository root.

## Add real deals

### Recommended: Google Sheets

Follow `GOOGLE-SHEETS-SETUP.md` and set your Sheet ID in `config.js`. The site reads the sheet when visitors load the page. Google Sheets remains your editing dashboard.

### Without Google Sheets

Click **Manage deals** in the website footer. Add/edit products, then click **Export deals.json**. Upload that file to the repository root and commit. Local edits alone are not visible to other visitors.

**Important:** The site deliberately starts with no invented live deals. You must supply verified products and authorized affiliate links. Use product images you have rights to use, and follow Amazon/Walmart affiliate rules. Prices may change. The website is not deployed automatically by this ZIP.

## Personalize text

Open `index.html` in any text editor and edit the intro, about-me paragraph, disclosure, and buttons. For social links, add your real profile URLs only after verifying them. The uploaded avatar is `justin-profile.png`.

## Hosting

GitHub Pages is free for qualifying projects, but its terms restrict certain commercial uses. Check GitHub's current policies before using it for a primarily affiliate-commerce website; choose an alternative host if your use isn't permitted.

# Deals With Justin — Free Affiliate Deals Website

A responsive, static website with Amazon/Walmart filters, search, categories, promo-code copying, affiliate links, and a browser-based deal editor.

## Launch for free with GitHub Pages

1. Sign up for a free GitHub account at https://github.com.
2. Create a **public** repository named `deals-with-justin` (or use `<username>.github.io` for a root site).
3. Upload **index.html**, **styles.css**, **app.js**, and **deals.json** into the repository's root folder (not the enclosing folder).
4. Open repository **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, branch **main**, folder **/(root)**, and save.
5. Visit `https://YOUR-USERNAME.github.io/deals-with-justin/` after GitHub finishes deploying.

**Important:** GitHub Pages has usage limits and restrictions; check its current terms to ensure your commercial/affiliate use is permitted. For a different free host, Cloudflare Pages supports static sites and GitHub deployments, subject to its terms and limits.

## Add real deals

1. Open the published website and click **Manage Deals**.
2. Delete the clearly labeled demo deals.
3. Enter your own product title, retailer, category, price, optional original price and promo code, your approved affiliate URL, and an image URL you are permitted to use.
4. Click **Save deal**. This changes only your own browser at first.
5. Click **Export deals.json**. In your GitHub repository, open `deals.json`, choose **Edit** (pencil icon), paste the contents of the downloaded file, and commit the change. Alternatively upload/replace the file using GitHub's upload workflow.
6. The public website will display the new deals after the deployment finishes. Refresh the page. If your browser still shows the old locally edited list, clear site storage or use a private window to see the public version.

### Important limitations

- The manager is a **local editor**, not a password-protected shared backend. It saves to your browser's localStorage; it does not publish automatically.
- Everyone can open the manager, but their edits affect only their own browser. Only people with access to your GitHub repository can publish changes to the public site.
- Prices, discounts, and sample listings are fictional demo content, not live offers. You must verify all prices and offers before publishing.
- Affiliate programs have rules about price freshness, images, links, trademarks, disclosures, and API use. Use only images and pricing that your agreements permit. Amazon may require approved API or other authorized tools for displaying certain product content.
- No automatic scraping or live price tracking is included.
- Free Google Fonts are loaded over the internet; fallback fonts are provided.

## Customization

Edit `index.html` to change the brand, hero wording, and disclosure. Edit `styles.css` for colors. The site works without build tools or paid services.

## Future upgrade

To publish directly from an admin dashboard across devices, add authentication and a database or connect a Google Sheet to a read-only feed. This starter intentionally avoids pretending that browser-local changes are globally published.

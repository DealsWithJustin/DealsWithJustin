# Google Sheets live editing (free)

This is the recommended way to run Deals With Justin. **You control the spreadsheet**; the website only reads it. There is no shared public editing permission.

1. Make a new Google spreadsheet. Rename the first tab exactly `Deals`.
2. Paste this header row into row 1 (each comma-separated header goes in its own column):
   `id,title,store,category,price,original,code,url,image,description,created`
3. Add one deal per row. Required: `title`, `price`, `url`. `store` can be Amazon, Walmart or Other. Use full HTTPS links. `created` can be a date like `2026-11-09`.
4. Choose **File → Share → Publish to web** and publish the `Deals` tab. Note: **anyone can read this published data**; do not put secrets or private information in the sheet. Do NOT grant public editing access.
5. Copy the spreadsheet ID from its URL: `https://docs.google.com/spreadsheets/d/SPREADSHEET_ID/edit`.
6. Open `config.js` and replace the empty `googleSheetId` value with your spreadsheet ID. Commit/upload that file to your website hosting once.
7. Refresh the site. The site reads the spreadsheet on page load. Future edits to the spreadsheet appear on the website after refresh, sometimes with a short Google publishing delay.

## Important

- You can edit products, prices, promo codes, images, and affiliate links entirely through Google Sheets after setup. No code changes are required for individual deals.
- Google Sheets public CSV access is not a guaranteed real-time API; it can be cached, and Google may change its publishing behavior.
- Use permitted product images and comply with Amazon Associates and Walmart affiliate program policies, including their rules for prices and content freshness. Never publish unverified discounts.
- The on-page Manage Deals form is an optional *local JSON editor* and **does not write back to Google Sheets**. When connected, edit the sheet instead.
- If you need an authenticated, on-site editor with one-click publishing, that requires a backend, authentication, and additional setup.

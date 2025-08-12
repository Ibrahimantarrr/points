
# S1 Submissions (Render Static Site)

This site has two pages:
- **index.html** — submission form (posts to Google Apps Script)
- **dashboard.html** — read-only table of submissions (loads JSON from Apps Script)
- **thanks.html** — redirect page after submission

## Endpoint
Current Apps Script endpoint:
```
https://script.google.com/macros/s/AKfycbyyUeT_LtM6VC-T8sMYouUmNL5DPS0IIr7nInzy8hvXJC230O0fK8YI-Mtu9X8KuKCXaQ/exec
```

## Deploy on Render (free)
1. Create a new GitHub repo and add these three files.
2. On Render → **New → Static Site**, connect the repo.
3. Settings:
   - **Build command:** *(leave blank)*
   - **Publish directory:** `/`
4. Deploy. Your site URL will be shown after a minute.

## Test
- Open `/index.html`, submit a test entry.
- Check your Google Sheet gets a new row.
- Open `/dashboard.html` to see it appear.

If the dashboard fails to load (CORS), tell me and I’ll provide a JSONP version.

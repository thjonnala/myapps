# Thiru Apps

A single-file static landing page (HTML + React via CDN — no build step) that lists all Thiru Apps as clickable tiles, plus **About Us** and **Contact Us** pages.

## Run it

Just open `index.html` in a browser. Or serve it locally:

```powershell
# from this folder
python -m http.server 8000
# then visit http://localhost:8000
```

## Add your own background image

Drop your image at:

```
assets/background.jpg
```

The page uses it automatically as the home background. If the file is missing,
a matching dark teal/blue gradient is shown as a fallback. (To use a different
filename, edit the `url("assets/background.jpg")` line in the `<style>` block.)

## Apps listed (each tile opens in a new tab)

| App | URL |
|-----|-----|
| Hyderabad Online Shopping | https://www.Hyderabadonlineshopping.com |
| Market Monitor | https://marketmonitor.thiruapps.com |
| Shopping | https://shopping.thiruapps.com |
| Astro | https://astro.thiruapps.com |
| AI Services | https://aiservices.thiruapps.com |
| Demo | https://demo.thiruapps.com |
| POC | https://poc.thiruapps.com |

To add/edit apps, change the `APPS` array near the top of the `<script>` block in `index.html`.

## Deploy

Because it's fully static, you can host it on GitHub Pages, Netlify, Vercel,
Azure Static Web Apps, or any web server — just upload `index.html` (and the
`assets/` folder if you add a background image).

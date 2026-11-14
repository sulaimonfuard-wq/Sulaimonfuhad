# Sulaimon Fuhad: Book Marketing & Launch Consultant

Static website for https://fuhadsulaimon.vercel.app/ (no build step).

## Files
- `index.html`: the whole site (HTML, CSS and a small script)
- `images/`: image files (the page embeds its own images; `og.jpg` and `sulaimon-fuhad.jpg` are used for social previews and search data)
- `robots.txt`, `sitemap.xml`: SEO files
- `vercel.json`: caching and security headers

## Before going live
- Contact form: open `index.html`, find `FORM SETTINGS`, and paste your Web3Forms access key (free at web3forms.com) and your email address.
- After deploying, submit `https://fuhadsulaimon.vercel.app/sitemap.xml` in Google Search Console.

## AI chat assistant
The "Ask a question" button works in two modes:
- **Without setup:** it answers common questions from a built-in FAQ (no cost).
- **With Claude:** in Vercel, open Project > Settings > Environment Variables, add `ANTHROPIC_API_KEY` (from console.anthropic.com), then redeploy. The function `api/chat.js` then answers any question in plain language using only the facts in its prompt. Set a monthly spend limit in the Anthropic console.

## Deploy
Connect this repository to Vercel (Framework preset: Other, no build command, output directory: root).
Every push to `main` redeploys the site.

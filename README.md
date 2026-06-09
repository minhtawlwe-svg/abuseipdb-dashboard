# AbuseIPDB Intelligence Dashboard

A modern, **fully client-side** dashboard for visualising [AbuseIPDB](https://www.abuseipdb.com/)
bulk IP-range scan results. Drop in a CSV and get an instant verdict, smart insights,
a risk pie chart, score distribution, and a searchable/sortable table.

**Everything runs in your browser — no data is ever uploaded.**

## Live demo
Loads bundled `sample-results.csv` automatically so you can try it with one click.

## Use it with your own data
1. Open the site (or `index.html` locally).
2. Drag your `abuseipdb-results.csv` onto the page, or click **Load CSV**.
3. Explore: filter chips (All / Reported / Suspicious / Malicious), search,
   click a pie slice or stat card to filter, click an IP to copy it, **Export** the
   filtered rows.

### CSV format
Header row plus these columns (extra columns are ignored):

```
IP,AbuseScore,Reports,Country,LastReported,ISP,UsageType
```

This is exactly what the companion PowerShell scanners produce. The scanner
scripts and any API keys are **not** part of this repo by design.

## Features
- Auto **verdict banner** + plain-language **smart insights**
- Interactive **donut** risk breakdown (hover + click-to-filter)
- Score-distribution bars, top-countries, animated stat cards
- Search, multi-filter, column sorting, copy-IP, export-filtered-CSV
- Slide-in help guide, responsive, offline, zero dependencies

## Deploy
Static site — no build step. Works on Vercel, Netlify, GitHub Pages, or any static host.
On Vercel: import the repo, framework preset **Other**, no build command, output = root.

## License
MIT

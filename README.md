# DIO Deals

Nationwide online deal finder for phones, tablets, and laptops.

The source package is `dio-deals-source.zip`. The GitHub Actions workflow unpacks it, runs the Worker smoke tests, and deploys only the public website files to GitHub Pages. The optional API Worker and database are separate Cloudflare resources; they are not deployed by GitHub Pages.

See the included package README for setup, privacy, affiliate disclosure, and Cloudflare deployment instructions. Deal listings come from an external aggregator and do not represent every local store in the United States. Prices and availability can change.

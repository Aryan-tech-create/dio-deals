# DIO Deals

DIO Deals is a responsive, installable storefront for discovering current online offers. It reads active listings from DealBuffalo's documented public JSON API, supports search, category filters and saved offers, and refreshes every five minutes while the page is open.

## Deploy

The site is published from this repository with GitHub Actions. In the repository, open **Settings → Pages** and choose **GitHub Actions** as the build and deployment source if it is not already selected. Then open **Actions → Publish DIO Deals** and confirm the latest run succeeds.

The default project site URL is:

`https://aryan-tech-create.github.io/dio-deals/`

Every push to `main` redeploys the public site. The workflow copies only `index.html`, `privacy.html`, `disclosure.html`, `manifest.webmanifest`, and `icon.svg` into its Pages artifact.

## Custom domain

A custom domain has not been attached yet because DIO's owner has not provided the exact domain name. Once a domain is owned and the parent/guardian managing its registrar account confirms the hostname, add it under **Settings → Pages → Custom domain**.

For a subdomain such as `www.example.com`, the usual DNS record is a CNAME from `www` to `aryan-tech-create.github.io`. For an apex domain such as `example.com`, GitHub Pages uses its documented A/AAAA records. Follow the current GitHub Pages instructions shown for the exact domain and enable Enforce HTTPS once available. DNS changes can take time to propagate.

## Deal data and limitations

- Listings come from DealBuffalo's documented public feed, which aggregates selected online offers. This is not a directory of every physical store or every local deal across all 50 states.
- Prices, availability, shipping and terms can change; always confirm with the retailer.
- Saved offers and the click counter currently live only in the visitor's browser.
- The Owner view is a local demonstration, not a password-protected or shared analytics dashboard.
- No DIO affiliate program is connected and this version does not report purchases or commissions. Real conversion tracking requires an approved affiliate program and a secured backend.
- Restricted or unsafe product listings are filtered from the visible feed.

A parent or guardian should manage domain purchases and any business, affiliate, tax or payment accounts that require an adult account holder. Never put passwords, payment details or secret tokens in the repository.

## Privacy and disclosure

Read [Privacy](privacy.html) and [Affiliate disclosure](disclosure.html). DealBuffalo's [API documentation](https://dealbuffalo.com/llms.txt) describes the upstream feed and its click-tracking links.

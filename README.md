# Reframed website

Static site for the Reframed iOS app by Bowtie Technology: landing page, privacy policy, and support page. Served by GitHub Pages from the `main` branch root.

- `index.html`: landing page
- `privacy/index.html`: privacy policy (App Store Connect Privacy Policy URL)
- `support/index.html`: support and FAQ (App Store Connect Support URL)
- `assets/`: stylesheet and images

Plain HTML and one CSS file. No build step, no cookies, no analytics, and no external fonts or scripts. Keep it that way so the site matches the app's privacy promise.

To preview locally: `python3 -m http.server` in this folder, then open http://localhost:8000.

When the privacy policy changes, update the "Last updated" date on the page.

## Custom domain (optional)

To serve the site from a subdomain such as `reframed.bowtietechnology.com`, add a DNS `CNAME` record pointing `reframed` to `bowtietech.github.io`, add a `CNAME` file to this repo containing `reframed.bowtietechnology.com`, then set the custom domain and enable "Enforce HTTPS" in the repo's Settings > Pages. Update the URLs in App Store Connect afterwards.

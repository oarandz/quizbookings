# The Woodsman's Quiz — complete upload package

## Which files are included?
- index.html: your supplied index(27).html, with the View Live Quiz button.
- live.html: the live-quiz page you supplied immediately before index(27).html.
- icons/: the generated Woodsman's Q icon in browser and home-screen sizes.
- manifest.webmanifest: app name, icon and launch settings.
- .nojekyll: static GitHub Pages configuration.

Both supplied HTML files are preserved exactly apart from added icon/manifest metadata. The existing theme colour on the live page is preserved. The View Live Quiz button opens live.html beside index.html. The home-screen app launches the booking page.

## Upload to GitHub
1. Unzip the package.
2. In your website repository, choose Add file → Upload files.
3. Upload the CONTENTS of the unzipped folder to your publishing folder, replacing index.html and live.html. Keep the icons folder intact. Upload the files, not the ZIP or an extra enclosing folder.
4. Commit the changes. Keep your existing GitHub Pages setup if it already works. Otherwise use Settings → Pages → Deploy from a branch → main → /(root) → Save. If your publishing folder is /docs, upload everything into that folder instead.
5. Keep any existing CNAME file for your custom domain.
6. Visit the HTTPS site after publishing, refresh, and check View Live Quiz.

Official guide: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Home-screen icon
Open the published site in Safari on iPhone/iPad and use Share → Add to Home Screen. On Android use your browser's Add to Home screen / Install option when offered. Existing shortcuts may retain their old icon until removed and added again.

## Existing services
No build step or new API key is needed. The supplied Supabase connections, backend functions, host sign-in, realtime subscriptions and notification settings remain unchanged. The existing backend must remain available; this package does not create or migrate it. Internet access is required. No offline booking or caching of customer/finance responses is added.

Verification: HTML source preservation, JavaScript syntax, local asset references, icon dimensions and archive contents. Live submissions, host sign-in, realtime data and GitHub deployment have not been tested or performed.

# The Woodsman's Quiz — GitHub upload package

## Upload
1. Unzip the download on your computer.
2. Open your existing website repository on GitHub and choose **Add file → Upload files**.
3. Upload the CONTENTS of this folder: `index.html`, `manifest.webmanifest`, the `icons` folder and `.nojekyll`. Keep the icons inside their folder. Replace the existing index.html. Do not upload the ZIP itself or place these files inside an extra github-package folder.
4. Commit the changes. If your repository already publishes its root through GitHub Pages, keep that setup.
5. Otherwise go to **Settings → Pages**, choose **Deploy from a branch**, choose your uploaded branch (usually `main`) and **/(root)**, then Save. If your existing Pages source is `/docs`, upload the same contents there instead.
6. Open the HTTPS website address shown by GitHub Pages when publishing finishes. Refresh the page to pick up the new icon.

GitHub documentation: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Home-screen icon
On iPhone/iPad, open the published site in Safari and use Share → Add to Home Screen. On Android, use the browser's Add to Home screen / Install option when available. Installation menus vary by browser. Existing home-screen shortcuts may retain their old icon; remove and add the shortcut again if necessary.

## Included
- Latest website, including restored background/logo, forecast dates and divider, jackpot comparisons and expanded weekly summary.
- PNG icons at 32, 180, 192 and 512 pixels.
- App manifest with relative URLs, so it works under a GitHub repository path or a custom domain.
- Existing background, logo and booking sound remain embedded in the HTML.

No build step, npm install, GitHub Actions configuration or new API key is needed. Keep any existing CNAME file if you use a custom domain.

## Existing services
This is the website front end. It retains the supplied Supabase connection and existing notification integration; it does not create or migrate a database. The existing backend functions and permissions must remain available. Bookings, finance, charts and external fonts need an internet connection. This package does not add offline booking or cache customer/finance responses.

The package has been checked for JavaScript syntax, icon dimensions and local asset links. Live booking submissions and deployment to your GitHub account have not been tested or performed.

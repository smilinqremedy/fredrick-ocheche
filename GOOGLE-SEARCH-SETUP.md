# Deployment and Google Search setup

This portfolio has been prepared for search discovery, but Google cannot index a local ZIP file. The site must first be deployed to a public HTTPS address.

## 1. Publish the portfolio for free with GitHub Pages

1. Open the `smilinqremedy/my-portoflio` repository on GitHub.
2. Upload the updated project files from this ZIP to the repository (or replace the repository contents).
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. Wait for GitHub Pages to publish the site. The likely project URL is `https://smilinqremedy.github.io/my-portoflio/`; use the exact URL GitHub displays.

## 2. Finish the site URL metadata

After the site is live, update the JSON-LD on `index.html` with the exact public URL in the Person `url` property. Update the social preview image URLs to absolute HTTPS URLs, for example:

`https://YOUR-PUBLISHED-SITE/assets/images/profile.jpg`

Do not use `ocheche.dev` unless you own that domain and have connected it to GitHub Pages.

## 3. Google Search Console

1. Visit https://search.google.com/search-console/
2. Add a **URL prefix** property using the exact published HTTPS URL.
3. Verify ownership using one of the methods Google offers. For GitHub Pages, the HTML file or HTML tag method may be practical.
4. Once the site is live, create a `sitemap.xml` containing the exact home and projects page URLs, then add its path to `robots.txt`.
5. Submit the sitemap in Search Console.
6. Use **URL Inspection** to request indexing for the home page and `projects.html`.

## 4. Important expectations

- Search indexing can take days or longer; it is not immediate.
- A successful indexing request does not guarantee indexing or a high ranking.
- Google AI Overviews are generated at Google's discretion. Structured data helps describe the site but does not guarantee an AI Overview.
- Keep your name, biography, project descriptions and links accurate and consistent across your website and public profiles.
- Only link to social accounts that you control.

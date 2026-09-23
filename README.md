# SFSBT Services website

A lightweight, responsive, single-page website for SFSBT Services Private Limited, built from the supplied brochure.

## Run locally

No package installation is required. Serve this folder with any static web server. For example, with Python available:

```powershell
python -m http.server 8000
```

Then open `http://localhost:8000` in a browser. Opening `index.html` directly also works, but a local server better reflects deployment behavior.

## Production build

There is no compile step or dependency bundle. Publish the project root to a static host such as Netlify, Cloudflare Pages or an existing web host. Keep the `assets/` directory alongside `index.html`, `styles.css` and `main.js`. After deployment, replace the canonical URL and sitemap URL if the production domain differs from `https://ifsdurgapur.netlify.app/`.

## Project structure

- `index.html` — semantic page content, metadata, contact links and structured data
- `styles.css` — responsive layout, colors, typography, components and reduced-motion support
- `main.js` — accessible mobile navigation and current footer year
- `assets/` — brochure images used by the site
- `robots.txt`, `sitemap.xml` — basic search engine discovery files
- `PROGRESS.md` — source analysis and implementation log

## Dependencies

No runtime or build dependencies. The site uses native HTML, CSS and JavaScript, and system font fallbacks.

## Assets used

- `assets/sfsbt-logo.jpg` — organization logo from the brochure
- `assets/site-team.jpg` — brochure image used in the home hero and social preview
- `assets/fire-system.jpg` — brochure fire equipment image
- `assets/water-treatment.jpg` — brochure water treatment image

The source brochure is retained in the project root. The exported, unused brochure images are also retained under `assets/` for future content: `image2.jpeg`, `image3.jpeg`, `image5.jpeg` and `image6.jpeg`.

## Content needing confirmation or replacement

- Confirm that `ifsdurgapur.netlify.app` is the preferred public domain. Update the canonical URL, Open Graph URL, JSON-LD URL and `sitemap.xml` together if not.
- Confirm the scope represented by the brochure's brief service labels `TPI` and `ETP/STP/WTP plant environmental and water treatment`; the page keeps these as listed and flags the missing scope.
- Confirm whether the structural stability service's stated “certification” is within SFSBT's authorized offering before publication.
- The brochure lists LinkedIn, Facebook and Instagram without profile URLs. Social links are omitted until URLs are supplied.
- Confirm the preferred formatting and availability of the two listed phone numbers.
- The brochure suggests a QR code but supplies no code or destination-specific QR asset; none has been invented.
- Consider replacing the brochure's small JPEG logo with a high-resolution SVG or transparent PNG for crisp display at larger sizes.

## Future integrations

- Add a real enquiry endpoint (for example a serverless function or configured form provider) if a web form is wanted; the current contact actions open the visitor's email or phone application directly.
- Add approved social profile links and a map link/embed once the official URLs and preferred location pin are confirmed.

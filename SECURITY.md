# Security Policy

## Security model

PlainResume is a static, single-file web app with no server side at all.

- **No server, no database, no analytics.** The app is served as static HTML and never sends your resume anywhere. There are no external requests at runtime.
- **Local storage only.** Your resume text and settings are saved in your browser's local storage so you can pick up where you left off. Clearing site data removes everything.
- **Share links carry the document.** The "Copy link" button encodes your resume text into the URL fragment. Anyone with the link can read that resume, so treat a share link like the document itself. The fragment is never sent to the hosting server by the browser.
- **Rendering is escaped.** All user text passes through an HTML-escaping function before it is rendered, and template and color inputs are validated against allowlists. Share-link payloads are size-capped before decoding.
- **Content Security Policy.** The page ships a CSP meta tag that blocks objects, form posts, and external connections as defense in depth.

## Supported versions

Only the latest version on the `master` branch and the live site at https://jc-965.github.io/PlainResume/ are supported.

## Reporting a vulnerability

If you find a way to execute script from resume text, a share link, or local storage, that is a real vulnerability and we want to know.

- Preferred: open a private report through [GitHub security advisories](https://github.com/Jc-965/PlainResume/security/advisories/new).
- Alternative: open a regular issue if the problem is not sensitive.

Please include the input text or link that triggers the problem and the browser you used. You should hear back within a week.

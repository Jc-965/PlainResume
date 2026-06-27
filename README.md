<div align="center">

# Onepage

### Plain text in. Polished resume out.

Onepage turns the resume you can already write in a text box into a clean, print ready document. No account, no fifty field form, no build step, and no file upload. It is a single HTML file that runs entirely in your browser.

[![License: MIT](https://img.shields.io/badge/license-MIT-2563eb?style=flat-square)](LICENSE)
[![Build](https://img.shields.io/badge/build-no%20build%20step-22c55e?style=flat-square)](#run-it-locally)
[![Dependencies](https://img.shields.io/badge/dependencies-zero-22c55e?style=flat-square)](#whats-inside)
[![Source](https://img.shields.io/badge/source-one%20HTML%20file-8b5cf6?style=flat-square)](index.html)
[![Tech](https://img.shields.io/badge/vanilla-HTML%20%7C%20CSS%20%7C%20JS-f59e0b?style=flat-square)](#whats-inside)
[![Privacy](https://img.shields.io/badge/data-100%25%20in%20your%20browser-0ea5e9?style=flat-square)](#privacy-by-design)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-ec4899?style=flat-square)](#contributing)

<img src="assets/onepage-hero.png" alt="The Onepage editor showing plain text on the left and a live, formatted resume on the right" width="900">

<sub>Type or paste on the left. Watch a formatted, one page resume build itself on the right.</sub>

</div>

---

## Why people like it

Most resume builders make you pour your experience into dozens of tiny inputs, then lock the good export behind a subscription, and keep a copy of your data on their servers. Onepage takes the opposite path. You write the way you think, the parser does the formatting, and nothing ever leaves the page.

| | Typical resume builder | Onepage |
| --- | --- | --- |
| Sign up | Required | None |
| Where your data lives | On their servers | Only in your browser |
| Input style | Dozens of form fields | Plain text you paste or type |
| Export | Often paywalled | Free, through the browser print dialog |
| Hosting | Their site only | One file you can self host anywhere |
| Dependencies | Many | Zero |

## From a messy paste to a finished resume

This is the part that feels like magic. Drop in something rough, with uneven spacing, lowercase labels, and dates glued to job titles. Onepage reads the structure and rebuilds it as a clean, aligned resume in real time.

<div align="center">
  <img src="assets/onepage-messy.png" alt="Messy unformatted text on the left becoming a clean Jake style resume on the right" width="860">
</div>

The text on the left can be as plain as this:

```text
Mira Vale
mira.vale@example.com | https://code.example/mira | (555) 010-2486 | Portland, OR
Product engineer focused on thoughtful AI tools and fast web platforms

EXPERIENCE
Software Engineering Intern | May 2025 - Aug 2025
Northwind Labs | Remote
- Reduced dashboard load time 32% by cleaning up duplicate API calls
```

There is no special markup to memorize. A few light conventions, listed in [Writing tips](#writing-tips), help the parser when your input gets unusual.

## Features

- **Live preview.** Every keystroke updates the page right away.
- **Seven templates.** Switch the entire look with one dropdown, then fine tune the font and accent color.
- **Messy paste support.** Dates, locations, bullets, degree lines, and contact rows get cleaned up for you.
- **Print ready export.** Export through the browser print dialog, so the text stays selectable and friendly to an [applicant tracking system](https://en.wikipedia.org/wiki/Applicant_tracking_system).
- **Click to source.** Select something in the preview and Onepage jumps to the matching line in the editor.
- **Shareable links.** Your resume can be packed into the URL, so sending the link recreates the document.
- **Local autosave.** Close the tab, reopen it later, and pick up from the last text you wrote.
- **Keyboard friendly and zoomable.** Adjust text size, zoom the page, or fit it to the pane.

<div align="center">
  <img src="assets/onepage-elegant.png" alt="The same resume rendered in the Elegant serif template next to its plain text source" width="880">
  <br>
  <sub>The same content, restyled in the Elegant template. The source text never changes.</sub>
</div>

## Templates

Seven directions, from quiet and modern to classic and academic.

- **Modern.** Clean sans serif with accent section rules.
- **Minimal.** Airy spacing and a softer editorial feel.
- **Compact.** Dense layout for resumes that must stay on one page.
- **Elegant.** Serif type with centered headings and subtle accents.
- **Computer Modern.** Styled after the [Computer Modern](https://en.wikipedia.org/wiki/Computer_Modern) family from LaTeX, for an academic look.
- **Jake's.** A centered name layout inspired by the popular [Jake's Resume](https://github.com/jakegut/resume) format used across the CS community.
- **Jake Sans.** The same practical structure with a modern sans serif finish.

Each template pairs with your choice of font and accent color.

## Try it now

Onepage is one file, so there is nothing to install.

1. Download or clone the repository.
2. Open `index.html` in any modern browser.
3. Start typing, or load a sample from the toolbar.

### Run it locally

Opening the file directly works for most things. For the full experience, including share links, serve it over a tiny static server:

```bash
git clone https://github.com/YOUR_USERNAME/onepage.git
cd onepage
python3 -m http.server 4173
```

Then open `http://127.0.0.1:4173`.

### Deploy anywhere

Because the app is static, you can host it for free in a couple of minutes on any of these:

- [GitHub Pages](https://pages.github.com)
- [Netlify](https://www.netlify.com)
- [Vercel](https://vercel.com)
- [Cloudflare Pages](https://pages.cloudflare.com)

Upload `index.html` (and the `assets` folder if you want the preview images) and you are live.

## Writing tips

You do not need a special syntax, but these conventions give the parser a clearer signal:

- Put the candidate name on the first line.
- Put contact details on the second line.
- Use section labels like `EXPERIENCE`, `Projects`, or `Skills:`.
- For a role, write `Title | Dates`, then `Company | Location` on the next line.
- Start a line with `-` when you want an exact bullet.
- Use `Label: value` for skill groups, for example `Languages: TypeScript, Python, SQL`.

## What the parser cleans up

Onepage is built for real pasted resumes, not only perfect examples. It can:

- Detect date ranges even when the spacing is inconsistent.
- Move dates and locations into a tidy right aligned column.
- Turn loose achievement lines into bullets inside experience and project sections.
- Recognize common education patterns, including schools, degrees, coursework, and graduation dates.
- Identify emails, phone numbers, and portfolio style links as contact details.

## Privacy by design

Onepage runs entirely in the browser. Your resume text is kept in local storage for convenience, and a shared resume is encoded into the link you copy. There is no server, no database, and no analytics.

One nice side effect: bookmarking the page is a real save button. As long as you have not cleared browser storage, reopening the site brings back the last resume you edited.

## What's inside

```text
.
|-- index.html   # The whole app: markup, styles, parser, renderer, and samples
|-- assets/      # Screenshots used in this README
|-- README.md    # You are here
`-- LICENSE      # MIT license
```

No frameworks, no bundler, no package install. Just open the file.

## Roadmap

- Sharper print tuning across every browser.
- More one page spacing controls.
- Optional section reordering.
- Import and export helpers for plain text and Markdown.
- Live template thumbnails in the picker.

## Contributing

Small, focused improvements are very welcome. Since this is a single file app, changes are easiest to review when they keep parser logic, rendering, and visual styling clearly separated. Open an issue to talk through larger ideas before sending a pull request.

## License and acknowledgements

Released under the [MIT License](https://opensource.org/license/mit). See [LICENSE](LICENSE) for the full text.

Template inspiration comes from the [Jake's Resume](https://github.com/jakegut/resume) layout and the [Computer Modern](https://en.wikipedia.org/wiki/Computer_Modern) type family. Badges are generated by [Shields.io](https://shields.io).



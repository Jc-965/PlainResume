<div align="center">

# Onepage

### Plain text in. Polished resume out.

Onepage turns the resume you can already write in a text box into a clean, print ready document. No account, no fifty field form, no build step, and no file upload. It is a single HTML file that runs entirely in your browser.

[![Live demo](https://img.shields.io/badge/live%20demo-open%20the%20app-2563eb?style=for-the-badge)](https://jc-965.github.io/OnePage/)

<a href="https://jc-965.github.io/OnePage/"><img src="https://github.com/Jc-965/OnePage/releases/download/v1.0.0/onepage-hero.png" alt="The Onepage editor showing plain text on the left and a live, formatted resume on the right" width="900"></a>

<sub>Type or paste on the left. Watch a formatted, one page resume build itself on the right.</sub>

**[Open the live app](https://jc-965.github.io/OnePage/)**

</div>

---

## Why its better

Most resume builders make you pour your experience into dozens of tiny inputs, then lock the good export behind a subscription, and keep a copy of your data on their servers. Onepage takes the opposite path. You write the way you think, the parser does the formatting, and nothing ever leaves the page.

| Dimension | Typical resume builder | Onepage |
| :--- | :--- | :--- |
| **Account** | Sign up required | None, ever |
| **Your data** | Stored on their servers | Stays in your browser |
| **Input style** | Dozens of tiny form fields | Plain text you paste or type |
| **Formatting** | Manual drag, click, and resize | Automatic, on every keystroke |
| **Export** | Often behind a paywall | Free, through the browser print dialog |
| **Templates** | Limited on the free tier | Seven, switchable instantly |
| **Hosting** | Their site only | One file you can host anywhere |
| **Dependencies** | Many | Zero |

## From raw text to a structured resume

This is the part that feels like magic. Drop in something rough, with uneven spacing, lowercase labels, missing bullets, and dates glued to job titles. Onepage reads the structure and rebuilds it as a clean, aligned resume in real time.

<table>
<tr>
<th align="left">Raw text you paste</th>
<th align="center">Structured resume you get</th>
</tr>
<tr>
<td valign="top">
<pre>
rowan pike
rowan.pike@example.com  (555) 010-9134  Oakland CA
software engineer / platform and product
summary
Software engineer building web apps, data
workflows, and internal platforms.
EXPERIENCE
Acme Cloud, San Francisco   Software Engineer   2022 - Now
rebuilt billing pipeline with Postgres, Redis, Node.
reduced invoice mismatch from 3.8% to 0.9%.
owned React admin console and service runbooks.
PROJECTS
release desk      2024
combined PRs, deploy status, and incidents.
SKILLS
languages TypeScript, Go, Python, SQL
backend Node, FastAPI, Postgres, Redis
</pre>
</td>
<td valign="top" align="center">
<img src="https://github.com/Jc-965/OnePage/releases/download/v1.0.0/resume-jakesans.png" alt="The same content rebuilt as a clean, aligned resume in the Jake Sans template" width="430">
</td>
</tr>
</table>

<sub>Left: text dropped straight into the editor. Right: the Jake Sans template, parsed and aligned automatically. Same words, zero manual formatting.</sub>

There is no special markup to memorize. A few light conventions, listed in [Writing tips](#writing-tips), help the parser when your input gets unusual.

## One source, every template

Pick a direction with one dropdown, then fine tune the font and accent color. The text you wrote never changes, only the styling around it.

<table>
<tr>
<td align="center"><img src="https://github.com/Jc-965/OnePage/releases/download/v1.0.0/resume-modern.png" alt="Modern template" width="210"><br><sub><b>Modern</b></sub></td>
<td align="center"><img src="https://github.com/Jc-965/OnePage/releases/download/v1.0.0/resume-elegant.png" alt="Elegant template" width="210"><br><sub><b>Elegant</b></sub></td>
<td align="center"><img src="https://github.com/Jc-965/OnePage/releases/download/v1.0.0/resume-minimal.png" alt="Minimal template" width="210"><br><sub><b>Minimal</b></sub></td>
<td align="center"><img src="https://github.com/Jc-965/OnePage/releases/download/v1.0.0/resume-jakesans.png" alt="Jake Sans template" width="210"><br><sub><b>Jake Sans</b></sub></td>
</tr>
</table>

## Features

- **Live preview.** Every keystroke updates the page right away.
- **Seven templates.** Switch the entire look with one dropdown, then fine tune the font and accent color.
- **Messy paste support.** Dates, locations, bullets, degree lines, and contact rows get cleaned up for you.
- **Print ready export.** Export through the browser print dialog, so the text stays selectable and friendly to an [applicant tracking system](https://en.wikipedia.org/wiki/Applicant_tracking_system).
- **Click to source.** Select something in the preview and Onepage jumps to the matching line in the editor.
- **Shareable links.** Your resume can be packed into the URL, so sending the link recreates the document.
- **Local autosave.** Close the tab, reopen it later, and pick up from the last text you wrote.
- **Keyboard friendly and zoomable.** Adjust text size, zoom the page, or fit it to the pane.

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

## Try it

Use it right now, nothing to install:

**[Open the live app](https://jc-965.github.io/OnePage/)**

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
|-- README.md    # You are here
`-- LICENSE      # MIT license
```

No frameworks, no bundler, no package install. Just open the file. The screenshots in this README are hosted as [release assets](https://github.com/Jc-965/OnePage/releases/tag/v1.0.0), so the repository tree stays to a single HTML file plus docs.

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

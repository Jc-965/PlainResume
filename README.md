<div align="center">

# PlainResume

### Plain text in. Polished resume out.

PlainResume is a free, open-source resume builder. It turns the resume you can already write in a text box into a clean, print-ready PDF. No account, no fifty-field form, no build step, and no file upload. It is a single HTML file that runs entirely in your browser.

[![Live demo](https://img.shields.io/badge/live%20demo-open%20the%20app-2563eb?style=for-the-badge)](https://jc-965.github.io/PlainResume/)

[![MIT license](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/Jc-965/PlainResume?style=flat&color=f5b301)](https://github.com/Jc-965/PlainResume/stargazers)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-8a63d2)](CONTRIBUTING.md)
[![Zero dependencies](https://img.shields.io/badge/dependencies-zero-1f883d)](#whats-inside)

<a href="https://jc-965.github.io/PlainResume/"><img src="https://github.com/Jc-965/PlainResume/releases/download/v1.0.0/onepage-hero.png" alt="The PlainResume editor showing plain text on the left and a live, formatted resume on the right" width="900"></a>

<sub>Type or paste on the left. Watch a formatted, one-page resume build itself on the right.</sub>

**[Open the live app](https://jc-965.github.io/PlainResume/)**

</div>

---

## Why it's better

Most resume builders, including resume.io, Zety, and Canva, make you pour your experience into dozens of tiny inputs, then lock the good export behind a subscription, and keep a copy of your data on their servers. PlainResume takes the opposite path. You write the way you think, the parser does the formatting, and nothing ever leaves the page.

| Dimension | Typical resume builder | PlainResume |
| :--- | :--- | :--- |
| **Account** | Sign up required | None, ever |
| **Your data** | Stored on their servers | Stays in your browser |
| **Input style** | Dozens of tiny form fields | Plain text you paste or type |
| **Formatting** | Manual drag, click, and resize | Automatic, on every keystroke |
| **Export** | Often behind a paywall | Free, through the browser print dialog |
| **Templates** | Limited on the free tier | Seven, switchable instantly |
| **Hosting** | Their site only | One file you can host anywhere |
| **Dependencies** | Many | Zero |

If you have used the popular [Jake's Resume](https://github.com/jakegut/resume) LaTeX template on Overleaf, the Jake's template here gives you that exact look with no LaTeX, no compiler, and no signup.

## From raw text to a structured resume

This is the part that feels like magic. Drop in something rough, with uneven spacing, lowercase labels, missing bullets, and dates glued to job titles. PlainResume reads the structure and rebuilds it as a clean, aligned resume in real time.

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
<img src="https://github.com/Jc-965/PlainResume/releases/download/v1.0.0/resume-jakesans.png" alt="The same content rebuilt as a clean, aligned resume in the Jake Sans template" width="430">
</td>
</tr>
</table>

<sub>Left: text dropped straight into the editor. Right: the Jake Sans template, parsed and aligned automatically. Same words, zero manual formatting.</sub>

There is no special markup to memorize. A few light conventions, listed in [Writing tips](#writing-tips), help the parser when your input gets unusual.

## One source, every template

Pick a direction from a dropdown with live thumbnail previews, then fine-tune the font and accent color. The text you wrote never changes, only the styling around it.

<table>
<tr>
<td align="center"><img src="https://github.com/Jc-965/PlainResume/releases/download/v1.0.0/resume-modern.png" alt="Modern template" width="210"><br><sub><b>Modern</b></sub></td>
<td align="center"><img src="https://github.com/Jc-965/PlainResume/releases/download/v1.0.0/resume-elegant.png" alt="Elegant template" width="210"><br><sub><b>Elegant</b></sub></td>
<td align="center"><img src="https://github.com/Jc-965/PlainResume/releases/download/v1.0.0/resume-minimal.png" alt="Minimal template" width="210"><br><sub><b>Minimal</b></sub></td>
<td align="center"><img src="https://github.com/Jc-965/PlainResume/releases/download/v1.0.0/resume-jakesans.png" alt="Jake Sans template" width="210"><br><sub><b>Jake Sans</b></sub></td>
</tr>
</table>

## Features

- **Live preview.** Every keystroke updates the page right away.
- **Seven templates.** Switch the entire look from a dropdown with live thumbnails, then fine-tune the font and accent color.
- **Messy paste support.** Dates, locations, bullets, degree lines, and contact rows get cleaned up for you.
- **True-to-preview PDF export.** The exported PDF matches the preview page for page, including where each page cuts. Text stays selectable and friendly to an [applicant tracking system](https://en.wikipedia.org/wiki/Applicant_tracking_system).
- **Click to source.** Select something in the preview and PlainResume jumps to the matching line in the editor.
- **Shareable links.** Your resume can be packed into the URL, so sending the link recreates the document.
- **Local autosave.** Close the tab, reopen it later, and pick up from the last text you wrote.
- **Light and dark theme.** Follows your browser's color scheme, with a one-click toggle to override it.
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

**[Open the live app](https://jc-965.github.io/PlainResume/)**

## Writing tips

You do not need a special syntax, but these conventions give the parser a clearer signal:

- Put the candidate name on the first line.
- Put contact details on the second line.
- Use section labels like `EXPERIENCE`, `Projects`, or `Skills:`.
- For a role, write `Title | Dates`, then `Company | Location` on the next line.
- Start a line with `-` when you want an exact bullet.
- Use `Label: value` for skill groups, for example `Languages: TypeScript, Python, SQL`.

## What the parser cleans up

PlainResume is built for real pasted resumes, not only perfect examples. It can:

- Detect date ranges even when the spacing is inconsistent.
- Move dates and locations into a tidy right-aligned column.
- Turn loose achievement lines into bullets inside experience and project sections.
- Recognize common education patterns, including schools, degrees, coursework, and graduation dates.
- Identify emails, phone numbers, and portfolio-style links as contact details.

## Privacy by design

PlainResume runs entirely in the browser. Your resume text is kept in local storage for convenience, and a shared resume is encoded into the link you copy. There is no server, no database, and no analytics. See [SECURITY.md](SECURITY.md) for the full security model.

One nice side effect: bookmarking the page is a real save button. As long as you have not cleared browser storage, reopening the site brings back the last resume you edited.

## What's inside

```text
.
|-- index.html       # The whole app: markup, styles, parser, renderer, and samples
|-- sitemap.xml      # Search engine sitemap for the live site
|-- README.md        # You are here
|-- CONTRIBUTING.md  # How to contribute
|-- SECURITY.md      # Security model and reporting
`-- LICENSE          # MIT license
```

No frameworks, no bundler, no package install. Just open the file. The screenshots in this README are hosted as [release assets](https://github.com/Jc-965/PlainResume/releases/tag/v1.0.0), so the repository tree stays to a single HTML file plus docs.

## Roadmap

- Sharper print tuning across every browser.
- More one-page spacing controls.
- Optional section reordering.
- Import and export helpers for plain text and Markdown.
- More templates, including two-column layouts.

## Contributing

Small, focused improvements are very welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) for how the single file is organized and what makes a change easy to review. Open an issue to talk through larger ideas before sending a pull request.

## Support the project

If PlainResume helped you land an interview or saved you a subscription, a star helps other job seekers find it.

[![Star this repo](https://img.shields.io/badge/star-this%20repo-f5b301?style=for-the-badge&logo=github)](https://github.com/Jc-965/PlainResume)

## License and acknowledgements

Released under the [MIT License](https://opensource.org/license/mit). See [LICENSE](LICENSE) for the full text.

Template inspiration comes from the [Jake's Resume](https://github.com/jakegut/resume) layout and the [Computer Modern](https://en.wikipedia.org/wiki/Computer_Modern) type family. Badges are generated by [Shields.io](https://shields.io).

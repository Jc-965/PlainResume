# Contributing to PlainResume

Thanks for wanting to help. Small, focused improvements are very welcome.

## Running it locally

There is no build step. Clone the repo and open `index.html` in a browser. That is the whole app.

```bash
git clone https://github.com/Jc-965/PlainResume.git
cd PlainResume
open index.html
```

## How the single file is organized

Everything lives in `index.html`, in this order:

1. **Head and SEO tags.** Meta tags, social cards, and the content security policy.
2. **Styles.** App chrome first, then the resume paper and the seven templates, then the light theme overrides, then responsive and print rules.
3. **Markup.** The toolbar, the editor pane, the preview pane, and the help dialog.
4. **Parser.** Turns plain text into a structured resume object. Look for `parse` and the helpers around it.
5. **Renderer.** Turns that object into HTML. Look for `renderHTML`.
6. **Pagination.** Splits the preview into letter-size pages and keeps print output matching the preview. Look for `updatePaperLayout`.
7. **App wiring.** Event handlers, custom selects, theme handling, share links, and autosave.
8. **Samples.** The example resumes offered in the sample picker.

## Guidelines

- **Keep it one file with zero dependencies.** No frameworks, no bundlers, no external requests. This constraint is the point of the project.
- **Keep parser, rendering, and styling separate.** A change is easiest to review when it stays in one of those layers.
- **Escape everything.** All user text must go through `esc()` before it reaches `innerHTML`. If you add a new render path, escape it.
- **Test with messy input.** Load the "Messy paste" sample and make sure your change survives it. Check a one-page and a multi-page resume.
- **Check both themes and print.** Toggle light and dark, and confirm the print preview still matches the on-screen pages.

## Reporting bugs

Open an issue with the text you pasted (redact anything personal), the template you used, your browser, and what you expected to happen. A screenshot of the preview helps a lot.

## Bigger ideas

Open an issue first so we can talk through the design before you write code. Roadmap items in the README are a good place to start.

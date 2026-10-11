# Website

The site is a static GitHub Pages website. `index.html` contains the layout, styles, and language-switching behavior. Page copy lives in Markdown files under `content/` and is loaded directly by the browser; no translation API or build service is required.

## Editing content

German is the editorial source of truth in `content/de.md`. Each `## key` heading identifies a text field used by the page. Put the text for that field on the following line(s), for example:

```md
## hero.title
Technologie, die im Alltag funktioniert.

## hero.copy
Ich verbinde IT, Prozesse und Menschen — von der Idee bis zur Umsetzung in der Filiale.
```

When you send new German Markdown content, Codex updates `content/de.md` and translates the corresponding fields in `content/da.md`, `content/sv.md`, and `content/en.md` in the same change. Keep the existing keys; Codex can add keys and connect new sections when the page grows.

The language switcher loads one Markdown file at a time. German is the default for visitors who have not chosen a language; the selection is saved in their browser.

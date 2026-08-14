---
title: "Example Project"
date: 2026-01-01
pin: 1
description: "A one-sentence summary shown on the projects list page."
tech: ["JavaScript", "CSS"]
repo: "https://github.com/yourusername/example-project"
live: ""
image: "/images/projects/example.png"
---
This is an example project write-up — plain markdown, rendered with `marked`. Fenced code blocks render as a terminal-style window, handy for install commands.

## Field notes

- `tech` — array of tags shown as small pills on both the list and detail page. Leave as `[]` or omit for none.
- `repo` — link to source, shown with a GitHub icon next to the title. Omit or leave `""` to hide the "repo" link entirely.
- `live` — link to a hosted/deployed version, shown with an external-link icon. Omit or leave `""` to hide the "live" link — useful for things with no hosted site, like a native app.
- `pin` — optional number. Set it to pin this project to the top of `/projects`, sorted lowest-first (`pin: 1` comes before `pin: 2`), and it'll show a small pin icon on its card. Leave it blank or delete the line for a normal, unpinned project — those sort by `date`, newest first.
- `image` — optional path to an image under `public/images/` (e.g. `/images/projects/your-image.png` — put the actual file there first). Renders to the left of the write-up on the detail page; on mobile it floats left and the text wraps around it. Leave blank or omit for no image. This example points at `/images/projects/example.png`, a placeholder graphic — swap it for a real image or delete the line.

## How to use this

This file is both a working example and a reference — it lives in `content/projects/` and renders at `/projects/example-project`. To add your own project, create a new `.md` file in `content/projects/`; the filename (minus `.md`) becomes the URL, e.g. `my-project.md` → `/projects/my-project`. Fill in the frontmatter fields above, then write the details below the `---`. `/projects` picks it up automatically the next time you run `npm run build` — no routes or other files need touching. Delete this file once you don't need the example anymore, or edit it into your first real project.

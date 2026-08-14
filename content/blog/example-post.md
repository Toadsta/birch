---
title: "Example Post"
date: 2026-01-01
excerpt: "One or two sentences shown on the /blog list page under the title and date."
tags: ["example"]
pin: 1
image: "/images/blog/example.png"
---
This is an example post — plain markdown, rendered with `marked`. Headings, links, lists, bold/italic, and fenced code blocks (rendered as a terminal-style window) all work.

## Field notes

- `tags` — array of tags shown as small pills, on both the list page and next to the title on the post itself. Leave as `[]` or omit for none.
- `pin` — optional number. Set it to pin this post to the top of `/blog`, sorted lowest-first (`pin: 1` comes before `pin: 2`), and it'll show a small pin icon on its list entry. Leave it blank or delete the line for a normal, unpinned post — those sort by `date`, newest first.
- `image` — optional path to an image under `public/images/` (e.g. `/images/blog/your-image.png` — put the actual file there first). Renders to the left of the post on the detail page; on mobile it floats left and the text wraps around it. Leave blank or omit for no image. This example points at `/images/blog/example.png`, a placeholder graphic — swap it for a real image or delete the line.

## How to use this

This file is both a working example and a reference — it lives in `content/blog/` and renders at `/blog/example-post`. To add your own post, create a new `.md` file in `content/blog/`; the filename (minus `.md`) becomes the URL, e.g. `my-new-post.md` → `/blog/my-new-post`. Fill in `title`, `date` (`YYYY-MM-DD`, controls sort order), and `excerpt`, then write the post below the `---`. `/blog` picks it up automatically the next time you run `npm run build` — no routes or other files need touching. Delete this file once you don't need the example anymore, or edit it into your first real post.

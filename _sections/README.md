# Blog sections

Each file in this folder is one section that shows up in the blog sidebar
(e.g. Investing, Life). The sidebar, the section's landing page, and its URL
are all generated automatically from the file below — you don't touch any
config, layout, or CSS.

## Add a new section (one file, ~5 lines)

1. Create a file here, e.g. `_sections/travel.md`:

   ```yaml
   ---
   title: Travel          # label shown in the sidebar + page heading
   category: travel       # the slug that ties posts to this section
   order: 3               # position in the sidebar (low = higher up)
   ---
   ```

2. Tag any post into the section by adding the matching `category` to its
   front matter:

   ```yaml
   ---
   layout: post
   title: "Two weeks in Japan"
   category: travel
   ---
   ```

That's it. The new section appears in the sidebar with a live post count, and
its page is served at `/travel/` (derived from the filename).

## Remove or rename a section

- Remove: delete the file. (Update any posts that used its `category`.)
- Rename the label: change `title`.
- Reorder: change `order`.
- Change the URL: rename the file (`travel.md` → `/travel/`).

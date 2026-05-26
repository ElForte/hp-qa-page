# Hello! Project Fan Site

A static fan site for Hello! Project, deployable on GitHub Pages.

## Structure

```
hello-project/
├── index.html       ← Main site (index + post viewer)
├── posts.json       ← All post data (edit this to add content)
└── .nojekyll        ← Required for GitHub Pages
```

## Deploy to GitHub Pages

1. Create a new GitHub repository (e.g. `hello-project-site`)
2. Upload all files in this folder to the repository root
3. Go to **Settings → Pages**
4. Set **Source** to `Deploy from a branch` → `main` → `/ (root)`
5. Click **Save** — your site will be live in ~1 minute at:
   `https://YOUR-USERNAME.github.io/REPO-NAME/`

## Adding Posts

Edit `posts.json` and add entries to the `"posts"` array. Each post has:

```json
{
  "id": 13,
  "title": "[b]Group Name[/b] — Event Title",
  "subtitle": "Short description",
  "posted_on": "2024-12-01",
  "thumbnail": "https://your-image-url.com/thumb.jpg",
  "content": "Your text with [b]BB code[/b] support."
}
```

## Supported BB Code

| Tag | Result |
|-----|--------|
| `[b]text[/b]` | **Bold** |
| `[i]text[/i]` | *Italic* |
| `[u]text[/u]` | Underline |
| `[s]text[/s]` | ~~Strikethrough~~ |
| `[quote]text[/quote]` | Block quote |
| `[url=https://...]Label[/url]` | Hyperlink |
| `[list][*]item[/list]` | Bullet list |
| `[color=#hex]text[/color]` | Text with color |
| `[img]https://...[/img]` | Inline image |
| `[spoiler]text[/spoiler]` | Hidden text |

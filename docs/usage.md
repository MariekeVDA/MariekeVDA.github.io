---
layout: default
title: Usage
nav_order: 4
---

# Usage

Learn how to customise and extend this documentation site.

---

## Editing Pages

All pages are written in [Markdown](https://www.markdownguide.org/). To edit a page, open the corresponding `.md` file and make your changes.

```bash
# Example: edit the home page
nano index.md
```

### Front Matter

Every page begins with **front matter** – a YAML block between `---` delimiters that controls page metadata:

```yaml
---
layout: default
title: My Page Title
nav_order: 5
---
```

| Key | Description |
|-----|-------------|
| `layout` | Which Jekyll layout to use (use `default` for standard pages) |
| `title` | The page title shown in the browser tab and headings |
| `nav_order` | Controls the order of pages in the navigation |

---

## Adding a New Page

1. Create a new `.md` file, either in the root or in the `docs/` folder:

   ```bash
   touch docs/my-new-page.md
   ```

2. Add front matter at the top:

   ```yaml
   ---
   layout: default
   title: My New Page
   nav_order: 5
   ---
   ```

3. Write your content in Markdown below the front matter.

4. Commit and push – GitHub Pages rebuilds the site automatically.

---

## Updating Site Settings

Edit `_config.yml` to change global settings:

```yaml
title: My Project Docs
description: Documentation for my awesome project.
theme: jekyll-theme-minimal
```

> ⚠️ **Note:** Changes to `_config.yml` require a server restart when previewing locally (`Ctrl+C`, then `bundle exec jekyll serve`).

---

## Markdown Cheat Sheet

| Element | Syntax |
|---------|--------|
| Heading | `# H1`, `## H2`, `### H3` |
| Bold | `**bold text**` |
| Italic | `*italic text*` |
| Link | `[label](url)` |
| Image | `![alt](url)` |
| Code | `` `inline code` `` |
| Code block | ` ```language ``` ` |
| Blockquote | `> quote` |
| List | `- item` or `1. item` |
| Table | `\| col \| col \|` |

---

[← Installation](installation)

# qwaeng.github.io

Personal academic homepage of Wangcheng Qu (瞿王城), in English (`/`) and Chinese (`/zh/`).
Built with plain Jekyll and deployed by GitHub Pages.

## Editing content / 修改内容

All text lives in `_data/`. Each entry has an `en` and a `zh` version.

| File | Contents |
| --- | --- |
| `_data/profile.yml` | Name, role, bio, interests, education, email, links, photo |
| `_data/research.yml` | Publications and working papers (newest first) |
| `_data/talks.yml` | Conference presentations (newest first) |
| `_data/ui.yml` | Interface labels (menu, section titles) |
| `_posts/` | Blog posts: `YYYY-MM-DD-title.md`, add `lang: zh` or `lang: en` in the front matter |

Papers in `research.yml` are written once, in their own language (`language: zh` or `language: en`),
and shown that way on both versions of the site.

YAML is indentation-sensitive: list items (`- `) at the same level must line up exactly,
otherwise the GitHub Pages build fails. For Chinese text, keep each paragraph on one line.

PDFs go in `assets/` and are linked as `/assets/<file>.pdf`.
To show a photo, add it to `images/` and set `photo: /images/<file>` in `profile.yml`.

## Layout

- `_layouts/default.html`: page shell (head, metadata)
- Pages: `index.html`, `research.html`, `talks.html`, `blog.html`, plus the same under `zh/`
- `_includes/pages/*.html`: page bodies, shared by both languages
- `_includes/paper.html`: one publication entry
- `assets/css/main.css`: styles (light/dark themes via CSS variables)
- `assets/js/main.js`: theme toggle and scroll animations

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

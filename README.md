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

PDFs go in `assets/` and are linked as `/assets/<file>.pdf`.
To show a photo, add it to `images/` and set `photo: /images/<file>` in `profile.yml`.

## Layout

- `_layouts/default.html`: page shell (head, metadata)
- `_includes/home.html`: the homepage sections, shared by both languages
- `assets/css/main.css`: styles (light/dark themes via CSS variables)
- `assets/js/main.js`: theme toggle and scroll animations

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

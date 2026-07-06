# Yasemin Tosun — Academic Website

A Jekyll site (About, Publications, Research & Projects, Teaching, News, Contact) ready to host free on GitHub Pages.

## 1. Your repo is already set up
Repo: `https://github.com/yasemintosun91/yasemintosun.git`
Site URL once Pages is on: `https://yasemintosun91.github.io/yasemintosun/`

`_config.yml` in this project is already set to match:
```yaml
url: "https://yasemintosun91.github.io"
baseurl: "/yasemintosun"
```

## 2. Upload these files
**No command line needed:**
1. Go to https://github.com/yasemintosun91/yasemintosun
2. Click **uploading an existing file** (or **Add file → Upload files**).
3. Drag in every file and folder from this project (unzip it first), keeping the folder structure intact — `_layouts`, `_includes`, `_posts`, `assets`, etc. all need to land at the repo root, not nested in an extra folder.
4. Scroll down, commit directly to `main`.

**Or with git**, from inside the unzipped folder:
```bash
cd site
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/yasemintosun91/yasemintosun.git
git push -u origin main
```

## 3. Turn on GitHub Pages
1. In the repo, go to **Settings → Pages**.
2. Under "Build and deployment", set **Source** to `Deploy from a branch`.
3. Set **Branch** to `main`, folder `/ (root)`. Save.
4. Wait 1–2 minutes, refresh — your live URL (`https://yasemintosun91.github.io/yasemintosun/`) will appear at the top.

### Want a shorter URL instead?
If you'd rather have `https://yasemintosun91.github.io/` (no `/yasemintosun/` at the end), rename the repo to `yasemintosun91.github.io` in **Settings → General → Repository name**, then in `_config.yml` set `baseurl: ""` and commit.

## Editing content
All page content lives in plain Markdown/HTML files — no build step needed locally, GitHub builds it for you on every push.

| To change...              | Edit this file                    |
|----------------------------|------------------------------------|
| Bio / About page           | `index.md`                        |
| Publications               | `publications/index.md`           |
| Research & projects        | `research/index.md`               |
| Teaching                   | `teaching/index.md`               |
| Contact info               | `contact/index.md`                |
| Top nav (name, links)      | `_includes/topnav.html`           |
| Colors / fonts / spacing   | `assets/css/style.css`            |
| CV file                    | replace `assets/cv/Yasemin_Tosun_CV.pdf` with an updated file of the same name |
| Add a news post            | add a new file to `_posts/`, named `YYYY-MM-DD-title.md` |
| Add a real photo           | drop an image in `assets/images/` and uncomment the `<img>` line in the hero block in `index.md` |

## Preview locally (optional)
If you have Ruby installed:
```bash
bundle install
bundle exec jekyll serve
```
Then open `http://localhost:4000`. Not required — GitHub Pages builds it for you either way.

# dr-farhan.github.io

Professional academic website for **Syed Farhan Ahmad, PhD**, built with Jekyll and the Beautiful Jekyll theme structure.

## What was revised

- Fixed the `_config.yml` YAML indentation issue that prevented Jekyll from parsing the site.
- Replaced leftover template biography content with Farhan-focused academic profile content.
- Updated navigation, social links, homepage, research page, publications page, talks page, contact page, and supporting pages.
- Added a professional profile stylesheet at `css/profile.css`.
- Removed unused third-party CV and old template profile assets.
- Updated build instructions for GitHub Pages.

## Local build

Install Ruby and Bundler, then run:

```bash
bundle install
bundle exec jekyll serve
```

Open the local URL printed by Jekyll, usually `http://127.0.0.1:4000/`.

## Deploy on GitHub Pages

1. Create or use the repository named `dr-farhan.github.io` under the `dr-farhan` GitHub account.
2. Upload/push these files to the repository root.
3. In GitHub, go to **Settings → Pages**.
4. Choose **Deploy from a branch** and select the `main` branch with `/root` as the folder.
5. Visit `https://dr-farhan.github.io` after the Pages build finishes.

## Editing content

Most website text can be edited directly in:

- `index.html` — homepage
- `aboutme.html` — about page
- `research.md` — research overview
- `publications.md` — selected publications
- `talks.md` — talks and presentations
- `contact.md` — contact links
- `_config.yml` — site title, navigation, colors, social links, and metadata

## Notes

Update the Google Drive CV link in `_config.yml` if your CV URL changes. Add a GA4 measurement ID to `google_analytics` only if you want analytics enabled.

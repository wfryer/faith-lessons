# Faith Formation Lessons

**Live lessons index: [wfryer.github.io/faith-lessons](https://wfryer.github.io/faith-lessons/)**

Lesson pages for adult Sunday school and small group study, by Wes Fryer. Each lesson is a single self-contained HTML page in its own folder, and `index.html` at the top lists them.

## Layout

```
index.html                                  the lessons index
.nojekyll                                   tells GitHub Pages to serve files as they are
2026-11-08-spirit-of-justice-ch8/index.html Women of the Movement (Spirit of Justice, Chapter 8)
2026-11-08-1526-week18-creole-mutiny/index.html The Creole Mutiny of 1841 (Project 1526, Week 18)
```

Folder names start with the class date (year, month, day) so they sort in order. Each lesson folder holds one `index.html`, so its web address ends at the folder name.

## Adding a lesson

1. Make a new folder named with the date and a short topic, for example `2026-11-15-spirit-of-justice-ch9`.
2. Put the lesson page in it as `index.html`.
3. In the top-level `index.html`, copy one `<article class="lesson">` block, paste it above the others so the newest is first, and change the date, title, book line, short description and the `href` (the folder name followed by a slash).

## Publishing with GitHub Pages

1. Create a public repository, for example `faith-lessons`, and add these files. In the browser you can use Add file, then Upload files, and drag in the whole folder contents. Dragging folders keeps their structure.
2. In the repository, open Settings, then Pages. Under Build and deployment choose Deploy from a branch, pick the `main` branch and the `/ (root)` folder, and save.
3. After a minute or two the site is live at `https://wfryer.github.io/faith-lessons/`.

## Optional: use a subdomain such as lessons.wesfryer.com

1. At the place that manages DNS for wesfryer.com, add a CNAME record: name `lessons`, value `wfryer.github.io`.
2. In the repository, open Settings, then Pages, enter `lessons.wesfryer.com` under Custom domain, and save. GitHub adds a `CNAME` file to the repository for you.
3. When the certificate is ready, turn on Enforce HTTPS.

## Notes

- Lesson pages are prepared with help from an AI assistant. Facts are checked against the sources each page lists.
- License: not yet chosen.

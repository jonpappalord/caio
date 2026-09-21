# CAIO blog setup

The blog uses Jekyll's built-in post system.

## Publishing an article

1. Copy `_drafts/blog-article-template.md` into `_posts/`.
2. Rename it `YYYY-MM-DD-short-title.md`.
3. Replace the front-matter placeholders and write the article.
4. Put its images in `assets/img/blog/short-title/` and update the paths.
5. Commit the article and images. The article will automatically appear on `/blog/`.

Files kept in `_drafts/` are not published by the standard GitHub Pages build.

The article structure is inspired by research-oriented editorial posts: a plain-language summary, quick links, problem, approach, findings, implications, next steps, figures and further reading.

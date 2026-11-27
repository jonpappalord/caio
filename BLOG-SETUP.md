# CAIO blog setup

The blog uses Jekyll's built-in post system.

## Publishing an article

1. Copy `_drafts/blog-article-template.md` into `_posts/`.
2. Rename it `YYYY-MM-DD-short-title.md`.
3. Replace the front-matter placeholders and write the article.
4. Put its images in `assets/img/blog/short-title/` and update the paths.
5. Commit the article and images. The article will automatically appear on `/blog/`.

Files kept in `_drafts/` are not published by the standard GitHub Pages build.

## Publishing a video or audio resource

Copy `_drafts/blog-media-template.md` into `_posts/` and rename it using the
same `YYYY-MM-DD-short-title.md` convention. Set `media_type` to `youtube`,
`spotify`, `video`, or `audio`.

- YouTube and Spotify entries use `media_id`.
- Local MP4 and MP3 entries use `media_src`.
- Local videos may optionally use `media_poster`.

Multimedia resources are embedded directly in the blog index. They do not show
the “Read article” link. Ordinary posts without `media_type` continue to work
as before.

The article structure is inspired by research-oriented editorial posts: a plain-language summary, quick links, problem, approach, findings, implications, next steps, figures and further reading.

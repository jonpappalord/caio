---
layout: post
title: "Title of the multimedia resource"
subtitle: "A short description of the video or audio."
author: "Author or speaker name"
date: YYYY-MM-DD
category: "Talk"
description: "A short description for search engines and link previews."

# Choose one supported media type: youtube, spotify, video, or audio.
media_type: "youtube"

# YouTube and Spotify use the resource ID, not the complete URL.
media_id: "YOUTUBE_VIDEO_ID"

# Local audio and video instead use media_src. Remove it for YouTube/Spotify.
# media_src: "/assets/audio/file-name.mp3"
# media_src: "/assets/video/file-name.mp4"

# Optional preview image for a local video.
# media_poster: "/assets/img/video-preview.jpg"

media_title: "Accessible title describing the multimedia player"
---

{% include media-player.html type=page.media_type src=page.media_src id=page.media_id poster=page.media_poster title=page.media_title %}

Add any links, credits, transcript, or further reading below the player. This
content remains available on the post's own URL even though the blog index
embeds the multimedia resource directly.

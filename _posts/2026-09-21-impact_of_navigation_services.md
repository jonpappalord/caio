---
layout: post
title: "A clear, concise title stating the research outcome"
subtitle: "One sentence explaining the main finding and why it matters."
author: "Author name"
date: YYYY-MM-DD
category: "Research"
description: "A short description for search engines and link previews."
image: /assets/img/blog/article-slug/hero.jpg
image_alt: "Describe what the image shows for readers using screen readers."
image_caption: "Optional caption and image credit."
links:
  - label: "Paper"
    url: "https://doi.org/..."
  - label: "Code"
    url: "https://github.com/..."
  - label: "Data"
    url: "https://..."
---

Begin with two or three short paragraphs that establish the real-world problem, explain what was previously unknown, and state the central result in plain language. A reader should understand why the study matters without needing to read the paper first.

## The problem

Describe the phenomenon or policy challenge. Introduce only the technical concepts needed to understand the research question, and link to reliable background material where useful.

## What we studied

State the research question and briefly describe the data, experiment, model or simulation. Focus on the logic of the approach rather than reproducing the full Methods section of the paper.

<figure class="blog-figure">
  <img src="{{ '/assets/img/blog/article-slug/figure-1.png' | relative_url }}" alt="Describe the evidence shown in the figure.">
  <figcaption><strong>Figure 1.</strong> Explain what the reader should notice and provide a credit if required.</figcaption>
</figure>

## What we found

Present the main results in order of importance. Use concrete quantities where they help interpretation, explain uncertainty, and distinguish clearly between evidence and interpretation.

> Use a short pull quote only for the article’s central takeaway.

## Why it matters

Explain the implications for cities, AI systems, public policy or future research. Be explicit about who may benefit and about any limits on how broadly the findings apply.

## What comes next

Conclude with open questions, planned extensions or practical steps suggested by the research.

## Further reading

- [Full paper](https://doi.org/...)
- [Related CAIO publication]({{ '/publications/' | relative_url }})

<!--
Publishing workflow:
1. Copy this file into _posts/.
2. Rename it YYYY-MM-DD-short-title.md.
3. Replace all placeholder text and URLs.
4. Put images in assets/img/blog/short-title/.
5. Add meaningful alt text and captions.
6. Preview locally, then commit the post and its images.
-->

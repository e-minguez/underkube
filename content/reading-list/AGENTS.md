# Reading List Post Structure

This document defines the structure and conventions for weekly reading list posts in `content/reading-list/`.

## End-to-End Workflow

1. Fetch links from the **Raindrop.io `00-Current` collection** (collection ID `62152014`) using the Raindrop MCP tool.
2. Organize, write, and save the post file.
3. Process and place the header image.
4. Commit and push to git.
5. Generate social media posts.
6. Move all links from `00-Current` to `99-old` (collection ID `61362542`) in Raindrop.

---

## Source of Links

Links come from the Raindrop.io **`00-Current`** collection (ID `62152014`). Use `mcp__raindrop__list_raindrops` with `perPage: 50` and paginate as needed to retrieve all bookmarks.

After the post is published and social media posts are generated, move all links to **`99-old`** (ID `61362542`). Use `mcp__raindrop__bulk_edit_raindrops` with `operation: move` — if that fails (known API issue), fall back to individual `mcp__raindrop__bookmark_manage` updates, or do it manually in the Raindrop web app.

---

## Directory Structure
Posts MUST be stored in subdirectories organized by year:
`content/reading-list/YYYY/filename.md`
Example: `content/reading-list/2026/2026-02-22-what-edu-is-reading-this-week-feb-16-22-2026.md`

## File Naming Convention
Files should be named following the pattern:
`YYYY-MM-DD-what-edu-is-reading-this-week-month-day-range-YYYY.md`
Example: `2026-02-22-what-edu-is-reading-this-week-feb-16-22-2026.md`

## Front Matter
Every post must include the following YAML front matter:

```yaml
title: "What Edu is reading this week (Month Day - Day, Year)"
date: YYYY-MM-DDTHH:MM:SS+HH:MM
draft: false
slug: YYYY-MM-DD-what-edu-is-reading-this-week-month-day-range-YYYY
aliases:
  - /posts/YYYY-MM-DD-what-edu-is-reading-this-week-month-day-range-YYYY/
categories:
  - Reading
tags:
  - newsletter
  - links
  - tech
  - devops
  - security
  - linux
  - ai
  - kubernetes
```

*Note: Adjust tags based on the actual content (e.g., add `sdr`, `gaming`, etc.).*

## Body Structure

### 1. Introduction
A brief one or two sentence introduction summarizing the week's themes or personal highlights. **Avoid exaggerated language or clickbait-style words (e.g., do not use words like "massive").** Keep the tone professional and grounded.

### 2. Featured Image
Recent posts include a featured image located in `/static/images/`. Reference it using the following syntax immediately after the introduction:

`![alt-text](/images/image-filename.png)`

**Image Requirements:**
- **Format:** MUST be PNG.
- **Dimensions:** Maximum 1200 pixels width.
- **Optimization:** Optimized for the web to minimize file size.

**Naming Convention for Images:**
`YYYY-MM-DD-what-edu-is-reading-this-week-month-day-range.png`

**Processing:** Use `magick` to resize and strip metadata:
```bash
magick input.png -resize 1200x -strip -define png:compression-level=9 /path/to/static/images/YYYY-MM-DD-what-edu-is-reading-this-week-month-day-range.png
```

### 3. Categories (H2)
Organize links into logical categories using H2 headers. Common categories include:
- `## Cloud, Kubernetes & Infrastructure`
- `## AI, Agents & Tools`
- `## Linux & Systems`
- `## Development, Web & Tools`
- `## Gaming, Fun & Misc`

Add or adjust categories to match the week's content (e.g., `## Sandboxing & Security`, `## SDR, Hardware & Electronics`).

### 4. Link Format
Links should be formatted as a bulleted list:
`* [**Link Title**](URL) - A concise, high-signal description of the content.`

If there are multiple related links (e.g., an article and a discussion thread):
`* [**Main Link**](URL) / [**Discussion**](URL): Description.`

Group related links (e.g., a GitHub repo and its companion article, an official announcement and its analysis, multiple databases for the same tool) on a single bullet using the `/` separator.

### 5. Link Retrieval & Verification
When processing links:
- **No Hallucination:** If the content or title of a link cannot be successfully retrieved (e.g., due to tool failures, paywalls, or bot protection), **DO NOT** hallucinate or guess the title or description.
- **Manual Verification:** If a link's information is unavailable, list the URL in your response and ask the user to provide the title and description manually.

### 6. Section Separators (Optional)
For very long posts, use `***` or `---` to separate major thematic groups if H2 headers alone are insufficient.

---

## Git Workflow

After writing the post and placing the image, stage and commit both files:

```bash
git add content/reading-list/YYYY/filename.md static/images/image-filename.png
git commit -m "feat(reading-list): add <Month Day-Day Year> weekly post and optimize image"
git push
```

---

## Social Media Posts

After pushing, generate copy-paste-ready posts (no quotes) for all four platforms:

- **X / Bluesky** (≤280/300 chars): One catchy sentence summarising the highlights + the post URL.
- **Mastodon** (≤500 chars): Same sentence, expand into 4-5 emoji-prefixed bullet highlights + URL + relevant hashtags (`#tech #linux #ai` etc.).
- **LinkedIn**: 2-3 sentence intro + bulleted highlights (5-7 items) + full URL.

Base URL: `https://www.underkube.com/posts/<slug>/`

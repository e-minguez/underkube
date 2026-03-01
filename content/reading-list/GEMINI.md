# Reading List Post Structure

This document defines the structure and conventions for weekly reading list posts in `content/reading-list/`.

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

### 3. Categories (H2)
Organize links into logical categories using H2 headers. Common categories include:
- `## Cloud, Kubernetes & Infrastructure`
- `## AI, Agents & Tools`
- `## Linux & Systems`
- `## Development, Web & Tools`
- `## Gaming, Fun & Misc`

### 4. Link Format
Links should be formatted as a bulleted list:
`* [**Link Title**](URL) - A concise, high-signal description of the content.`

If there are multiple related links (e.g., an article and a discussion thread):
`* [**Main Link**](URL) / [**Discussion**](URL): Description.`

### 5. Section Separators (Optional)
For very long posts, use `***` or `---` to separate major thematic groups if H2 headers alone are insufficient.

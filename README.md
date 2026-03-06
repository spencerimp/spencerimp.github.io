# spencerimp.github.io

Personal tech blog powered by [Quartz v4](https://quartz.jzhao.xyz/). Deployed to GitHub Pages via GitHub Actions.

🌐 **Live site:** https://spencerimp.github.io

> After pushing to `main`, the build takes ~1–2 minutes. Track progress at:
> https://github.com/spencerimp/spencerimp.github.io/actions

## Setup

Requires Node.js 22+.

```bash
npm install
```

## Local preview

```bash
npx quartz build --serve
```

Then open http://localhost:8080.

## Write a new post

Create a file in `content/`:

```bash
# content/yyyy-mm-dd-my-post-title.md
```

Minimal front matter:

```yaml
---
title: My Post Title
date: 2026-03-06
tags: [python, ml]
---

Post content here.
```

Then add a wikilink to it in `content/index.md`:

```md
- [[yyyy-mm-dd-my-post-title|My Post Title]]
```

## Add images

Put images in `static/post_images/` and reference them in Markdown:

```md
![alt text](/post_images/my-image.png)
```

## Deploy

Push to `main` — GitHub Actions builds and deploys automatically.

### One-time GitHub setup

1. Go to your repo on GitHub
2. **Settings → Pages**
3. Under **Source**, select **GitHub Actions**
4. Save

After that, every push to `main` triggers a build (~1–2 min). Track progress at:
https://github.com/spencerimp/spencerimp.github.io/actions

## Configuration

- `quartz.config.ts` — site title, base URL, plugins, theme colors
- `quartz.layout.ts` — page layout and sidebar components

# Noble Adike’s Summer 2025 Research Blog

Welcome! This repo contains the source code for **my personal research website**, built with Jekyll + the Minimal theme. Inside you’ll find daily reflections, an overview of my summer project, and shout-outs to the mentors who helped me grow.

[🔗 View the live site → kingnaddy.github.io](https://kingnaddy.github.io)

Recruiters & collaborators, feel free to jump to:

- **Daily Reflections** – Track my learning curve and problem-solving approach  
- **About Me** – My background, core skills, and career interests  
- **Mentor Spotlights** – Meet the experts guiding my research  
- **Project Overview** – Goals, methods, and results of the summer work  

---


## 📂 Project Structure

```
├── _config.yml           ← Site settings
├── _layouts/             ← Custom layouts (default, post, mentor, about, project, home)
├── _posts/               ← Daily blog posts (YYYY-MM-DD-slug.md)
├── pages/                ← Standalone pages (about-*.md, my-blog.md, index.md)
├── assets/
│   ├── css/style.scss    ← Custom SCSS overrides
│   └── images/           ← Store profile, mentor, project, blog images here
└── README.md             ← This guide
```

---

## ⚙️ Configuration (`_config.yml`)

Open `_config.yml` and set:

```yaml
title: "YOUR NAME"  
description: "CEAMLS SAIRI Summer 2025 Research Site"  
remote_theme: pages-themes/minimal@v0.2.0  
plugins:
  - jekyll-remote-theme
future: true            
```

---

## 📝 Adding a New Blog Post

1. Create a file in `_posts/` named `YYYY-MM-DD-day-N.md` (e.g. `2025-06-12-day-6.md`).
2. Add Front Matter:

```yaml
---
layout: post
title: "Day N – YOUR TITLE"
date: YYYY-MM-DD
author: YOUR NAME
---
```

3. Write your post content following the structure below:

```markdown
### What I Learned
- …

### Blockers
- …

### Reflection
I feel…
```

---

## ✍️ Editing About Pages

Standalone pages live in `pages/`. Each uses a layout:

* **About Me** → `layout: about`
* **About My Mentors** → `layout: mentor`
* **About My Project** → `layout: project`

### Example `about-me.md`

```yaml
---
layout: about
title: About Me
permalink: /about-me.html

about:
  name: Noble Adike
  role: Sophomore, Computer Science Major at Howard University
  image: /assets/images/me.jpg
  linkedin: https://www.linkedin.com/in/noble-adike-2356b2324/
  bio: |
    I’m a sophomore at Howard University …
---
```

---

## 🖼️ Managing Images

* Put images in `assets/images/`
* Reference with:

```liquid
<img src="{{ '/assets/images/example.jpg' | relative_url }}" alt="Example">
```

---

## 💅 Custom Styles

Use `assets/css/style.scss`:

```scss
---
---
@import "{{ site.theme }}";

/* Your styles here */
.profile-card { /* ... */ }
.blog-toc a { /* ... */ }
```

---

## 🚀 Running Locally

```bash
bundle install
bundle exec jekyll serve --livereload
```

Preview at `http://localhost:4000`

---

## 📤 Deployment

Just push to `main`. GitHub Pages will build your site automatically.

---

## 🔎 Tips

* **Images:** Store in `assets/images`.
* **Blog TOC:** Posts are grouped into weeks automatically.
* **Layouts:** Add new layouts in `_layouts/`, use them via `layout:` in the front matter.
* **Front Matter:** Always include correct `date:` so posts sort and display properly.

---

Enjoy writing and sharing your journeys! 📚💼

---
layout: post
title:  "Setup and deploy Jekyll"
date:   2025-11-01 20:55:52 -0400
categories: jekyll setup
---

1. To get started

```bash
gem install bundler jekyll
jekyll new put-your-site-name-here
cd put-your-site-name-here
bundle exec jekyll serve
```

2. Go To [http://localhost:4000](http://localhost:4000)

3. To generate your site's static HTML

```bash
JEKYLL_ENV=production bundle exec jekyll build
```

4. Find generated HTML in `_site` directory



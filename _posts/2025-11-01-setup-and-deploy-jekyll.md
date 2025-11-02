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
    bundle exec jekyll serve [--verbose]
    ```

2. Go To [http://localhost:4000](http://localhost:4000)

6. To deploy to GitHub pages
    1. Create GitHub new repo and push code
    2. Add a CNAME record with my DNS service provider using github-username.github.io
    3. GitHub repo > Settings > Pages > Build and deployment > Branch
    4. Pages > Custom domain
    5. GitHub creates a CNAME file in the project root

3. To generate your site's static HTML

    ```bash
    JEKYLL_ENV=production bundle exec jekyll build [--verbose]
    ```

4. Find generated HTML in `_site` directory

5. To find default minima template files

    ```bash
    bundle show minima
    bundle info --path minima
    ```

6. To find minima version

    ```bash
    grep minima Gemfile
    gem "minima", "~> 2.5"
    ```



# Little Earth Solutions GitHub Pages Site

This is the GitHub Pages site for Little Earth Solutions, converted from the original website at [littleearthsolutions.net](https://littleearthsolutions.net).

## Setup Instructions

### 1. Enable GitHub Pages

1. Go to your repository settings on GitHub
2. Scroll down to the "Pages" section
3. Under "Source", select "Deploy from a branch"
4. Choose "main" branch and "/ (root)" folder
5. Click "Save"

### 2. Repository Structure

```
├── _config.yml              # Jekyll configuration
├── _layouts/                # Page layouts
│   ├── default.html
│   ├── post.html
│   ├── page.html
│   └── product.html
├── _includes/               # Reusable components
│   ├── social.html
│   ├── google-analytics.html
│   └── disqus_comments.html
├── _posts/                  # Blog posts
├── _products/               # Product pages
├── assets/css/              # Stylesheets
├── index.md                 # Home page
├── products.md              # Products listing
├── links.md                 # Links page
├── about.md                 # About page
└── blog.md                  # Blog listing
```

### 3. Customization

#### Update Site Information
Edit `_config.yml` to update:
- Site title and description
- Author information
- Social links
- Navigation menu

#### Add New Blog Posts
Create new files in `_posts/` with the format:
```markdown
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD
categories: [Category]
---

Your post content here...
```

#### Add New Products
Create new files in `_products/` with the format:
```markdown
---
layout: product
title: "Product Name"
version: "1.0.0"
github_url: "https://github.com/username/repo"
---

Product description...
```

### 4. Local Development

To run the site locally:

1. Install Jekyll:
   ```bash
   gem install jekyll bundler
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

3. Run the development server:
   ```bash
   bundle exec jekyll serve
   ```

4. Open [http://localhost:4000](http://localhost:4000) in your browser

### 5. Deployment

The site will automatically deploy to GitHub Pages when you push changes to the main branch. The site will be available at:
`https://littleearth.github.io/`

### 6. Custom Domain Setup

The site is configured to use the custom domain `www.littleearthsolutions.net`:

1. ✅ `CNAME` file created with `www.littleearthsolutions.net`
2. ✅ `url` setting updated in `_config.yml`
3. ⚠️ **DNS Configuration Required** (see below)

#### DNS Configuration Steps

To make `www.littleearthsolutions.net` work with GitHub Pages, you need to configure your DNS settings:

1. **Go to your domain registrar's DNS management panel** (where you bought littleearthsolutions.net)

2. **Add/Update these DNS records:**
   ```
   Type: CNAME
   Name: www
   Value: littleearth.github.io
   TTL: 3600 (or default)
   ```

3. **Optional - Redirect root domain to www:**
   ```
   Type: CNAME
   Name: @ (or leave blank for root)
   Value: www.littleearthsolutions.net
   TTL: 3600
   ```

4. **Enable HTTPS (Recommended):**
   - In your GitHub repository, go to Settings → Pages
   - Under "Custom domain", enter `www.littleearthsolutions.net`
   - Check "Enforce HTTPS" (available after DNS propagation)

5. **Wait for DNS propagation** (can take up to 24-48 hours)

#### Verification
- Visit `https://www.littleearthsolutions.net` to confirm it's working
- The site should show your GitHub Pages content

## Features

- ✅ Responsive design
- ✅ Blog with post categories
- ✅ Product showcase
- ✅ GitHub integration
- ✅ SEO optimized
- ✅ Social media links
- ✅ Search functionality (via GitHub)
- ✅ Comment system ready (Disqus)

## Original Website

This site is based on content from [littleearthsolutions.net](https://littleearthsolutions.net) and includes all the blog posts and product information from the original site.

## License

This site content is licensed under the same terms as the original Little Earth Solutions website.

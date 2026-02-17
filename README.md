# Eric Antonian - Personal Website

This is my personal website built with [Quarto](https://quarto.org/), featuring my CV and blog posts.

## Features

- CV/Resume as the homepage
- Blog with automatic post listing
- Automatic deployment to GitHub Pages via GitHub Actions
- Responsive design with the Cosmo theme

## Local Development

To preview the website locally:

```bash
quarto preview
```

To render the website:

```bash
quarto render
```

## Deployment

The website automatically deploys to GitHub Pages when changes are pushed to the main branch. The GitHub Actions workflow handles:

1. Checking out the repository
2. Setting up Quarto
3. Rendering the website
4. Deploying to GitHub Pages

## Adding Blog Posts

To add a new blog post:

1. Create a new directory in `blog/posts/` with the format `YYYY-MM-DD-post-title`
2. Create an `index.qmd` file in that directory
3. Add YAML frontmatter with title, author, date, categories, and description
4. Write your content in Markdown
5. Push to GitHub - the site will update automatically!

## Project Structure

```
├── _quarto.yml          # Main configuration
├── index.md             # CV/Homepage
├── blog/
│   ├── index.qmd        # Blog listing page
│   └── posts/           # Blog posts
├── styles.css           # Custom styling
└── .github/
    └── workflows/
        └── publish.yml  # Deployment workflow
```

## License

Content © Eric Antonian. All rights reserved.

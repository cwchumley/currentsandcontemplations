# Currents and Contemplations

A personal blog exploring thoughts, ideas, and experiences. Built with Hugo and hosted on GitHub Pages.

## About

This blog serves as a space for sharing insights, exploring ideas, and connecting with others who value deep thinking and authentic expression. The name "Currents and Contemplations" represents the flow of ideas and the deep thinking that goes into understanding the world around us.

## Technology Stack

- **Static Site Generator**: [Hugo](https://gohugo.io/)
- **Theme**: [PaperMod](https://github.com/adityatelange/hugo-PaperMod)
- **Hosting**: GitHub Pages
- **Deployment**: GitHub Actions (automatic)

## Local Development

To run this blog locally:

1. **Install Hugo** (Extended version recommended)
   ```bash
   # macOS with Homebrew
   brew install hugo
   
   # Or download from https://gohugo.io/installation/
   ```

2. **Clone the repository**
   ```bash
   git clone https://github.com/cchumley/currentsandcontemplations.git
   cd currentsandcontemplations
   ```

3. **Start the development server**
   ```bash
   hugo server -D
   ```

4. **View the site** at `http://localhost:1313`

## Adding Content

### New Blog Post
```bash
hugo new posts/my-new-post.md
```

### New Page
```bash
hugo new about.md
```

## Deployment

The site automatically deploys to GitHub Pages when changes are pushed to the `main` branch. The GitHub Actions workflow:

1. Builds the Hugo site
2. Optimizes assets
3. Deploys to GitHub Pages

## Site Structure

```
├── content/          # Blog posts and pages
├── layouts/          # Custom layouts (if any)
├── static/           # Static assets (images, etc.)
├── themes/           # Hugo themes
├── hugo.toml         # Site configuration
└── .github/          # GitHub Actions workflows
```

## License

This blog content is licensed under [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

## Contact

Feel free to reach out with comments, questions, or suggestions for future posts.

---

*Built with ❤️ using Hugo and PaperMod* 
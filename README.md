# 📝 My Notes

A public notes repository for sharing personal learnings, thoughts, and references. This repository uses GitHub Pages to display notes in a clean, accessible format.

## 🌐 Live Site

Visit the notes at: `https://neurofoo.github.io/notes/`

## 📚 Features

- **Static Site**: Built with pure HTML/CSS for fast loading and simple maintenance
- **GitHub Pages**: Automatically deployed using GitHub Actions
- **Responsive Design**: Mobile-friendly interface that works on all devices
- **Easy to Update**: Simply add new HTML files to the `notes/` directory and update the index

## 🏗️ Structure

```
.
├── index.html              # Main landing page with notes index
├── styles.css              # Shared stylesheet for all pages
├── notes/                  # Directory containing individual note pages
│   ├── getting-started.html
│   └── sample-note.html
├── .github/
│   └── workflows/
│       └── pages.yml       # GitHub Actions workflow for deployment
└── README.md
```

## ✍️ Adding New Notes

1. Create a new HTML file in the `notes/` directory (use `notes/sample-note.html` as a template)
2. Add a new card entry in `index.html` linking to your new note
3. Commit and push your changes
4. GitHub Actions will automatically deploy to GitHub Pages

## 🔒 Access Control

This repository is configured to restrict who can create pull requests and issues:

### Repository Settings Required

To ensure only you can create PRs and issues, configure the following in GitHub repository settings:

1. **General Settings** (`Settings > General`):
   - Set repository visibility to "Public" (to allow read access)
   
2. **Collaborators** (`Settings > Collaborators`):
   - Don't add any collaborators (only the owner has write access)

3. **Branch Protection** (`Settings > Branches`):
   - Set up branch protection rules for `main`/`master` branch
   - Require pull request reviews before merging (optional)
   - Restrict who can push to matching branches (owner only)

4. **Issues** (`Settings > General > Features`):
   - Keep Issues enabled (they're restricted by default to those with write access in some configurations)
   - Note: GitHub doesn't provide a direct way to prevent issue creation on public repos, but you can:
     - Use issue templates to guide reporting
     - Quickly close unwanted issues
     - Use GitHub Discussions instead for community interaction

5. **Pull Requests** (`Settings > General > Features`):
   - Keep Pull requests enabled
   - Anyone can create PRs on public repos, but only you can merge them

### Best Practices

- **Issues**: While public repos allow anyone to create issues, you maintain control over which ones to address
- **Pull Requests**: Public repos allow PRs from forks, but you control what gets merged
- **Discussions**: Consider enabling GitHub Discussions for community feedback while keeping Issues for your own tracking

## 🚀 Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the main branch. The GitHub Actions workflow (`.github/workflows/pages.yml`) handles the deployment process.

### Manual Deployment

You can also trigger a manual deployment from the Actions tab in GitHub.

## 📄 License

All rights reserved. Content is available for reading and reference.

## 🛠️ Technology Stack

- **HTML5** - Structure and content
- **CSS3** - Styling and responsive design
- **GitHub Pages** - Hosting
- **GitHub Actions** - Automated deployment
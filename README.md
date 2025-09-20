# ReadingPaper-HBM

A comprehensive collection of research paper readings and analysis focused on High Bandwidth Memory (HBM) technology, built as a static site using [mdBook](https://rust-lang.github.io/mdBook/).

## 📖 Read Online

The latest version is automatically published to GitHub Pages: **[https://cosmoswafer.github.io/ReadingPaper-HBM/](https://cosmoswafer.github.io/ReadingPaper-HBM/)**

## 🚀 Local Development

### Prerequisites

- [Rust](https://rustup.rs/) (for mdBook)
- [mdBook](https://rust-lang.github.io/mdBook/guide/installation.html)

### Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/cosmoswafer/ReadingPaper-HBM.git
   cd ReadingPaper-HBM
   ```

2. **Install mdBook:**
   ```bash
   cargo install mdbook
   ```

3. **Serve locally:**
   ```bash
   mdbook serve
   ```
   
   The book will be available at `http://localhost:3000`

4. **Build static files:**
   ```bash
   mdbook build
   ```
   
   Output will be in the `book/` directory.

## 📝 Content Structure

```
src/
├── SUMMARY.md              # Table of contents
├── introduction.md         # Welcome page
├── papers/                 # Paper reviews
│   ├── README.md
│   ├── hbm-fundamentals.md
│   └── performance-analysis.md
├── notes/                  # Research notes
│   └── README.md
└── references.md           # Citations and resources
```

## 🔄 Automatic Deployment

Changes to the `main` branch automatically trigger:
1. **Build**: mdBook generates static HTML
2. **Deploy**: Content is published to GitHub Pages

The deployment workflow is defined in `.github/workflows/deploy.yml`.

## ✏️ Contributing

1. Add new papers by creating `.md` files in the `src/papers/` directory
2. Update `src/SUMMARY.md` to include new chapters
3. Follow the established template format for consistency
4. Test locally with `mdbook serve` before committing

## 🏗️ Technology Stack

- **[mdBook](https://rust-lang.github.io/mdBook/)**: Static site generator for documentation
- **[GitHub Pages](https://pages.github.com/)**: Hosting platform  
- **[GitHub Actions](https://github.com/features/actions)**: Automated CI/CD pipeline

---

*A living document for HBM research insights and analysis.*
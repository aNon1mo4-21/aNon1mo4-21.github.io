# Site Maintenance: Building the Garden

*——automating the flow from thought to web* 🏗️

This site, **Abby's Wonderland**, is powered by **MkDocs** and the **Material theme**. It is designed to be a lightweight, version-controlled repository of my academic and technical growth.

## 📝 Maintenance Checklist

- [x] **Local Preview**: Running `mkdocs serve` to verify $\LaTeX$ rendering.
- [ ] **Automated Deploy**: Setting up GitHub Actions for seamless `gh-pages` updates.
- [ ] **Asset Optimization**: Compressing 3D meshes and high-res images for faster loading.
- [x] **Structure Audit**: Ensuring the `mkdocs.yml` navigation stays clean as the garden grows.

------

## 🚀 The Deployment Workflow

## 1. The Local Sandbox

I write in **Markdown** using VS Code or Obsidian. To see changes in real-time:

Bash

```
# Spin up the local dev server
mkdocs serve
```

*Access via `localhost:8000`.*

## 2. The Build Process

When a module (like a new CV research note) is complete, I build the static site:

Bash

```
mkdocs build
```

This converts all Markdown files, $\LaTeX$ math blocks, and code snippets into optimized HTML/CSS.

## 3. Shipping to the Web

I use **GitHub Pages** for hosting. The deployment is a single command:

Bash

```
mkdocs gh-deploy
```

------

## 🎨 Theme & Extensions

## **Material for MkDocs**

Chosen for its high-performance search, mobile responsiveness, and "Admonitions" (those useful callout blocks).

## **MathJax / KaTeX**

Essential for rendering the heavy lifting of **Mathematical Analysis** and **3DCV** equations.

YAML

```
# In mkdocs.yml
extra_javascript:
  - javascripts/mathjax.js
  - https://polyfill.io/v3/polyfill.min.js?features=es6
  - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
```

------

## 📂 Directory Structure

Plaintext

```
.
├── docs/
│   ├── math/          # Analysis, Linear Algebra
│   ├── coding/        # C++, Verilog, Python
│   ├── research/      # 3DCV & Embodied AI
│   └── index.md       # The "Digital Garden" landing page
├── mkdocs.yml         # Site configuration & Navigation
└── requirements.txt   # Python dependencies
```

------

## 💡 Future Enhancements

- **Interactive 3D**: Integrating `three.js` or `Gradio` components to showcase 3D reconstructions directly on the page.
- **Dark Mode Toggle**: For those late-night coding sessions in the Turing Class lab.
- **Search Optimization**: Better indexing for deep technical terms.

------

<p align="center">

<small>"A digital garden is never finished; it only evolves."</small>

</p>
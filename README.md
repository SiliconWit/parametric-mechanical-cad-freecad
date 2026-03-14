---
title: "Parametric Mechanical CAD with FreeCAD - Collaboration Guide"
description: "Contributing guide for Parametric Mechanical CAD with FreeCAD course content"
tableOfContents: true
sidebar:
  order: 999
---

# Parametric Mechanical CAD with FreeCAD

![Build](https://img.shields.io/badge/build-passing-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Contributors Welcome](https://img.shields.io/badge/contributors-welcome-orange)

**Read this course at:** [https://siliconwit.com/education/parametric-mechanical-cad-freecad/](https://siliconwit.com/education/parametric-mechanical-cad-freecad/)

A course on engineering design methodology using FreeCAD. Each lesson builds one complete mechanical mechanism with dimensions derived from kinematic analysis, manufacturing constraints, and engineering requirements. Covers slider crank, four-bar linkage, scissor lift, toggle clamp, pantograph, cam and follower, Geneva mechanism, scotch yoke, and Python scripting for advanced CAD.

## Lessons

| # | Title |
|---|-------|
| 1 | Slider Crank Mechanism |
| 2 | Four-Bar Linkage Mechanism |
| 3 | Scissor Lift Mechanism |
| 4 | Toggle Clamp Mechanism |
| 5 | Pantograph Mechanism |
| 6 | Cam and Follower Mechanism |
| 7 | Geneva Mechanism |
| 8 | Scotch Yoke Mechanism |
| 9 | Python Scripting for Advanced CAD |

## File Structure

```
parametric-mechanical-cad-freecad/
├── index.mdx
├── slider-crank-mechanism.mdx
├── four-bar-linkage-mechanism.mdx
├── scissor-lift-mechanism.mdx
├── toggle-clamp-mechanism.mdx
├── pantograph-mechanism.mdx
├── cam-and-follower-mechanism.mdx
├── geneva-mechanism.mdx
├── scotch-yoke-mechanism.mdx
├── python-scripting-advanced-cad.mdx
└── README.md
```

## How to Contribute

1. Fork the repository: [SiliconWit/parametric-mechanical-cad-freecad](https://github.com/SiliconWit/parametric-mechanical-cad-freecad)
2. Create a feature branch: `git checkout -b feature/your-topic`
3. Make your changes and commit with a clear message
4. Push to your fork and open a Pull Request against `main`
5. Describe what you changed and why in the PR description

## Content Standards

- All lesson files use `.mdx` format
- `<BionicText>` may be used in later content sections but not in lesson intro paragraphs
- Code blocks should include a title attribute:
  ````mdx
  ```python title="parametric_linkage.py"
  import FreeCAD
  doc = FreeCAD.newDocument("Linkage")
  ```
  ````
- Use Starlight components (`<Tabs>`, `<TabItem>`, `<Steps>`, `<Card>`) where appropriate
- Keep paragraphs concise and focused on practical application
- Include working FreeCAD scripting examples where relevant
- Mathematical notation uses LaTeX in MDX

## Local Development

Clone the main site repository and initialize submodules:

```bash
git clone --recurse-submodules <main-repo-url>
cd siliconwit-com
npm install
npm run dev
```

To test a production build:

```bash
npm run build
```

## License

This course content is released under the [MIT License](LICENSE).

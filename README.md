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

All commands below work on Linux, macOS, and Windows (using Git Bash, PowerShell, or Command Prompt with Git installed).

### For Team Members (with push access)

**First time setup (clone the repo once):**

```bash
git clone https://github.com/SiliconWit/parametric-mechanical-cad-freecad.git
cd parametric-mechanical-cad-freecad
```

**Every time you start working:**

```bash
git pull origin main
```

Always pull before making changes. This avoids conflicts with other contributors.

**After making your changes:**

```bash
git add .
git commit -m "Brief description of what you changed"
git push origin main
```

**If you get a push error** (someone pushed before you):

```bash
git pull origin main
```

Git will merge the changes automatically in most cases. If there is a conflict, Git will mark the conflicting lines in the file. Open the file, choose which version to keep, then:

```bash
git add .
git commit -m "Resolve merge conflict"
git push origin main
```

**Tips to avoid conflicts:**

- Always `git pull origin main` before you start working
- Push your changes as soon as you are done, do not hold onto uncommitted work for long
- Coordinate with other contributors so two people are not editing the same file at the same time

### For External Contributors (without push access)

1. Fork the repository: [SiliconWit/parametric-mechanical-cad-freecad](https://github.com/SiliconWit/parametric-mechanical-cad-freecad)
2. Clone your fork:
   ```bash
   git clone https://github.com/YOUR-USERNAME/parametric-mechanical-cad-freecad.git
   cd parametric-mechanical-cad-freecad
   ```
3. Make your changes and commit:
   ```bash
   git add .
   git commit -m "Brief description of what you changed"
   git push origin main
   ```
4. Open a Pull Request against `main` on the original repository
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

To preview the full site locally, clone the main site repository and initialize submodules:

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

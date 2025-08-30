# 📄 Islam AbdElhady — CV

[![CV PDF](https://img.shields.io/badge/Download-CV-blue)](https://islam-hady9.github.io/Islam-Abdelhady-CV/Islam_Abdelhady_CV.pdf)  
[![GitHub Pages](https://img.shields.io/badge/View%20Online-GitHub%20Pages-brightgreen)](https://islam-hady9.github.io/Islam-Abdelhady-CV/)

---

## 🚀 About
This repository contains the **LaTeX source code** of my personal **Curriculum Vitae (CV)**.  
It is built automatically with **GitHub Actions** and deployed to **GitHub Pages**, ensuring the latest version is always available online.

- ✨ Written in **LaTeX** using the [sb2nov RenderCV theme](https://github.com/sinaatalay/rendercv).  
- ⚙️ **CI/CD pipeline** powered by `latexmk` + GitHub Actions.  
- 🌐 Always up-to-date, hosted with **GitHub Pages**.  
- 🖥️ Optimized for **ATS** with `glyphtounicode` mappings.  

---

## 📥 Download / View

- **Direct PDF:** [Islam_Abdelhady_CV.pdf](https://islam-hady9.github.io/Islam-Abdelhady-CV/Islam_Abdelhady_CV.pdf)  
- **Landing Page:** [GitHub Pages Site](https://islam-hady9.github.io/Islam-Abdelhady-CV/)  

---

## 👀 Preview

![CV Preview](cv/assets/preview.png)

*(Preview of the first page — open the PDF for full details.)*

---

## 🛠 Repository Structure

```
.
├─ cv/                          # Main LaTeX sources
│  ├─ Islam_Abdelhady_CV.tex    # Final CV (your actual content in LaTeX)
│  ├─ sb2nov_base.tex           # Base template (reference, sb2nov RenderCV theme)
│  ├─ glyphtounicode.tex        # Unicode mapping to ensure ATS-friendly / machine-readable PDF
│  ├─ assets/                   # Images, previews (e.g., preview.png for README/landing page)
│  └─ build/                    # Temporary build artifacts (ignored in git, used by latexmk)
│
├─ dist/                        # ✅ Published to GitHub Pages (contains final PDF + site landing page)
│  ├─ Islam_Abdelhady_CV.pdf    # Generated CV (compiled from LaTeX)
│  └─ index.html                # Landing page with link(s) to download/view CV
│
├─ template/                    # Minimal LaTeX template for reuse
│  └─ minimal_template.tex      # Starter template for others to adapt their own CV
│
├─ tools/                       # Build tools and automation configs
│  ├─ Makefile                  # Build instructions (compile LaTeX, copy outputs, generate preview)
│  └─ latexmkrc                 # Config file for latexmk (defines build rules and settings)
│
├─ .github/workflows/           # GitHub Actions CI/CD definitions
│  └─ pages.yml                 # Workflow that builds the CV and deploys to GitHub Pages
│
├─ LICENSE                      # Licensing terms (MIT for template/tools, All Rights Reserved for CV content)
└─ README.md                    # Project overview, usage instructions, links to PDF/Pages
```

---

## 🔄 How It Works

1. **Edit** your CV in `cv/Islam_Abdelhady_CV.tex`.  
2. **Commit & Push** → GitHub Actions compiles the PDF.  
3. The workflow copies the PDF into `dist/` and **deploys** it to GitHub Pages.  
4. ✅ The CV is instantly live at:  
   - Root: [islam-hady9.github.io/Islam-Abdelhady-CV/](https://islam-hady9.github.io/Islam-Abdelhady-CV/)  
   - PDF: [Islam_Abdelhady_CV.pdf](https://islam-hady9.github.io/Islam-Abdelhady-CV/Islam_Abdelhady_CV.pdf)

---

## 📚 Reusing This Template

If you’d like to use this workflow for your own CV:

1. Fork this repo.  
2. Replace the contents of `cv/Islam_Abdelhady_CV.tex` with your own CV.  
3. Update `README.md` with your details.  
4. Push to `main`.  
5. Enable GitHub Pages → Source: GitHub Actions.  
6. Enjoy an always-up-to-date online CV 🎉.

---

## 📬 Contact

- 🌐 [LinkedIn](https://linkedin.com/in/islam-abd-elhady-323523211)  
- 🐙 [GitHub](https://github.com/islam-hady9)  
- 📧 [Email](mailto:eslamabdo71239@gmail.com)  

---

## 📄 Licensing

- The LaTeX **template** and **build workflow** are open-sourced under the [MIT License](LICENSE).
- The actual **CV content** (`Islam_Abdelhady_CV.tex`, `Islam_Abdelhady_CV.pdf`, `preview.png`)  
  is © 2025 Islam Abd-Elhady — all rights reserved.  
  You may view these files, but reuse or redistribution is not permitted.

---

💡 *This project shows how LaTeX + GitHub Actions + Pages can give you a professional, auto-updating, and easily shareable CV.*
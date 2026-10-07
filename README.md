# IBM Concert Workshop

<p align="center">
  <img src="docs/assets/images/ibm-logo.png" alt="IBM Logo" width="80"/>
</p>

<p align="center">
  <strong>Workshop técnico interactivo de IBM Concert — Plataforma Agentic de ITOps</strong><br/>
  <em>Interactive technical workshop for IBM Concert — Agentic ITOps Platform</em>
</p>

<p align="center">
  <a href="https://ibm-automation-spgi.github.io/concert-workshop/"><img src="https://img.shields.io/badge/docs-live-0043ce?style=flat-square&logo=readthedocs" alt="Docs"/></a>
  <img src="https://img.shields.io/badge/language-ES%20%7C%20EN-78a9ff?style=flat-square" alt="Bilingual"/>
  <img src="https://img.shields.io/badge/labs-7-198038?style=flat-square" alt="Labs"/>
  <img src="https://img.shields.io/badge/duration-4--5h-ff832b?style=flat-square" alt="Duration"/>
  <img src="https://img.shields.io/badge/IBM%20Concert-3.0.3-0f62fe?style=flat-square" alt="Concert"/>
</p>

---

## 📋 Descripción / Description

**ES:** Workshop práctico que guía a los participantes a través de todas las funcionalidades de [IBM Concert](https://www.ibm.com/products/concert), la plataforma agentic de ITOps que unifica observabilidad, protección, resiliencia y optimización.

**EN:** Hands-on workshop guiding participants through all features of [IBM Concert](https://www.ibm.com/products/concert), the agentic ITOps platform that unifies observability, protection, resilience and optimization.

---

## 🗂️ Laboratorios / Labs

| Lab | Módulo / Module | Duración / Duration |
|-----|-----------------|---------------------|
| 🚀 **Lab 0** | Prerequisitos / Prerequisites | 10 min |
| 🏠 **Lab 1** | Introducción a Concert / Introduction to Concert | 15 min |
| 🛡️ **Lab 2** | Concert Protect — CVEs, SBOM, Certificados | 25 min |
| 🔭 **Lab 3** | Concert Observe — APM, Trazas, Alertas | 20 min |
| ⚙️ **Lab 4** | Concert Resilience — Incidentes, Runbooks | 20 min |
| 📊 **Lab 5** | Concert Optimize — Right-Sizing, Costes | 15 min |
| 🔄 **Lab 6** | Concert Workflows — Automatización Low-Code | 15 min |

**Total: ~2 horas de laboratorio**

---

## 🚀 Inicio rápido / Quick Start

### Prerrequisitos / Prerequisites

```bash
python3 -m pip install -r requirements.txt
```

### Servir en local / Serve locally

```bash
mkdocs serve
# Abre / Open: http://localhost:8000
```

### Build estático / Static build

```bash
mkdocs build
# Output: site/
```

### Deploy a GitHub Pages

```bash
mkdocs gh-deploy
```

---

## 🌐 Idiomas / Languages

El workshop está disponible en **Español** (por defecto) e **Inglés**.  
The workshop is available in **Spanish** (default) and **English**.

El selector de idioma aparece en la cabecera de cada página.  
The language selector appears in the header of every page.

---

## 🏗️ Estructura del proyecto / Project structure

```
concert-workshop/
├── docs/
│   ├── index.es.md          # Home (Español)
│   ├── index.en.md          # Home (English)
│   ├── lab0/
│   │   ├── index.es.md      # Lab 0 - Español
│   │   └── index.en.md      # Lab 0 - English
│   ├── lab1/ … lab6/        # (same structure)
│   ├── assets/
│   │   └── images/          # Screenshots reales de IBM Concert
│   └── styles/
│       └── custom.css       # IBM Carbon tokens
├── mkdocs.yml               # MkDocs + Material + i18n config
└── requirements.txt         # Python dependencies
```

---

## 🛠️ Stack técnico / Tech stack

| Herramienta | Versión | Uso |
|-------------|---------|-----|
| [MkDocs](https://www.mkdocs.org/) | ≥ 1.5 | Generador de docs estáticas |
| [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) | ≥ 9.4 | Tema IBM-styled |
| [mkdocs-static-i18n](https://ultrabug.github.io/mkdocs-static-i18n/) | ≥ 1.2 | Soporte bilingüe ES/EN |
| [mkdocs-glightbox](https://blueswen.github.io/mkdocs-glightbox/) | ≥ 0.3 | Lightbox para screenshots |
| [Mermaid.js](https://mermaid.js.org/) | 10 | Diagramas de arquitectura |

---

## 📸 Screenshots

Todas las capturas de pantalla son **reales**, tomadas directamente del entorno de demostración de IBM Concert 3.0.3.

All screenshots are **real**, taken directly from the IBM Concert 3.0.3 demo environment.

---

## 👥 Autoría / Authors

**IBM Client Engineering — SPGI**

- Workshop diseñado para sesiones presenciales y remotas
- Entorno de demostración: IBM Concert 3.0.3

---

## 📄 Licencia / License

Copyright © 2026 IBM Corporation. All rights reserved.

Este material es para uso exclusivo en workshops y sesiones de formación autorizadas por IBM.  
This material is for exclusive use in IBM-authorized workshops and training sessions.

---
marp: true
theme: ctte-docs
paginate: true
math: katex
title: Product Documentation — <Your Product>
description: Versioned, multi-format docs with Marp
author: Technical Writing Team
footer: "Docs • 23f3000663@ds.study.iitm.ac.in"
---

<style>
/* @theme ctte-docs */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap');

section {
  font-family: Inter, system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
  font-size: 28px; line-height: 1.35; padding: 70px; color: #0f172a;
}
h1, h2, h3 { font-weight: 800; letter-spacing: -0.02em; }
h1 { font-size: 64px; margin: 0 0 12px; }
h2 { font-size: 44px; margin: 0 0 8px; }
h3 { font-size: 32px; }
code, pre { font-family: ui-monospace, SFMono-Regular, Menlo, monospace; }
a { color: #2563eb; text-decoration: none; } a:hover { text-decoration: underline; }

/* Slide accents */
.lead { background: linear-gradient(135deg,#eef2ff,#e0f2fe); }
.invert { color: #f8fafc; }
.invert h1, .invert h2, .invert h3 { color: #ffffff; }

/* Page numbers (enabled by `paginate: true`) */
section::after {
  content: attr(data-marpit-pagination) " / " attr(data-marpit-pagination-total);
  position: absolute; right: 32px; bottom: 24px;
  font-size: 18px; color: currentColor; opacity: 0.6;
}

/* Footer placement */
footer { position: absolute; left: 70px; bottom: 18px; font-size: 18px; opacity: 0.7; }

/* Background image readability */
.bg-mask::before {
  content: ""; position: absolute; inset: 0; background: rgba(0,0,0,0.38);
}
.bg-mask { color: #ffffff; }
</style>

<!-- _class: lead -->
# Product Documentation — <Your Product>

Version: v1.0  
Last updated: 20 Aug 2025  
Contact: **23f3000663@ds.study.iitm.ac.in**

- Single-source Markdown
- Export to HTML / PDF / PPTX
- CI-friendly

---

## Goals

- Keep docs versioned in Git.
- One source → many outputs.
- Reusable theme for all product docs.

<!--
style: |
  ul li { margin: 10px 0; }
-->

---

## Quick Start (local)

```bash
# Serve live (auto-reload)
npm run watch

# Export formats
npm run build:html
npm run build:pdf
npm run build:pptx

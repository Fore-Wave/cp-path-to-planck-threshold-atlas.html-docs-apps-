
cff-version: 1.2.0
message: "If you use this work, please cite it as below."
title: "The Planck Threshold — Visual Atlas"
abstract: >-
  An interactive, non-linear field guide to temporal order at the Planck scale,
  zitterbewegung, time crystals, and the emergence of macroscopic coherence.
  Companion to the MVRP / Fore-Wave open-science program.
type: software
authors:
  - family-names: Howell
    given-names: Evan
    affiliation: "Independent Researcher (Fore-Wave)"
url: "https://github.com/Fore-Wave"
repository-code: "https://github.com/Fore-Wave"
license: MIT
keywords:
  - Planck scale
  - zitterbewegung
  - time crystals
  - coherence
  - golden ratio
  - phyllotaxis
  - open science
  - interactive visualization
identifiers:
  - type: doi
    value: 10.5281/zenodo.18167536
    description: "Parent Zenodo dataset (MVRP Framework)"
preferred-citation:
  type: dataset
  title: "MVRP Framework: φ-Geometry Effects on Physical Coherence — Comprehensive Dataset"
  authors:
    - family-names: Howell
      given-names: Evan
  year: 2025
  publisher:
    name: Zenodo
  doi: 10.5281/zenodo.18167536
  url: "https://doi.org/10.5281/zenodo.18167536"

<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>The Planck Threshold — Visual Atlas</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { background: #070611; display: flex; align-items: center; justify-content: center; min-height: 100vh; font-family: -apple-system, BlinkMacSystemFont, sans-serif; }
    #__bundler_loading { position: fixed; bottom: 20px; right: 20px; font: 13px/1.4 -apple-system, BlinkMacSystemFont, sans-serif; color: #666; background: #fff; padding: 8px 14px; border-radius: 8px; box-shadow: 0 1px 4px rgba(0,0,0,0.12); z-index: 10000; }
    #__bundler_thumbnail { position: fixed; inset: 0; width: 100%; height: 100%; display: flex; align-items: center; justify-content: center; background: #070611; z-index: 9999; }
    #__bundler_thumbnail svg { width: 100%; height: 100%; object-fit: contain; }
    #__bundler_placeholder { color: #999; font-size: 14px; }
  </style>
  <noscript>
    <style>#__bundler_loading { display: none; }</style>
    <div style="position:fixed;bottom:12px;left:12px;font:13px/1.4 -apple-system,BlinkMacSystemFont,sans-serif;color:#999;background:rgba(255,255,255,0.9);padding:6px 12px;border-radius:6px;box-shadow:0 1px 4px rgba(0,0,0,0.08);z-index:10000;">
      This page requires JavaScript to display.
    </div>
  </noscript>
</head>
<body>
  <div id="__bundler_thumbnail">
    <svg viewBox="0 0 1200 800" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <radialGradient id="tcore" cx="50%" cy="46%" r="42%">
          <stop offset="0%" stop-color="#ffd27a"></stop>
          <stop offset="38%" stop-color="#ff4d97"></stop>
          <stop offset="70%" stop-color="#a06bff"></stop>
          <stop offset="100%" stop-color="#070611" stop-opacity="0"></stop>
        </radialGradient>
        <linearGradient id="tline" x1="0" y1="0" x2="1" y2="0">
          <stop offset="0" stop-color="#6a6dff"></stop><stop offset="0.5" stop-color="#a06bff"></stop><stop offset="1" stop-color="#34dfe0"></stop>
        </linearGradient>
      </defs>
      <rect width="1200" height="800" fill="#070611"></rect>
      <circle cx="600" cy="368" r="300" fill="url(#tcore)"></circle>
      <line x1="180" y1="368" x2="1020" y2="368" stroke="url(#tline)" stroke-width="3"></line>
      <circle cx="600" cy="368" r="64" fill="none" stroke="#ffd27a" stroke-width="3" opacity="0.85"></circle>
      <g fill="#34dfe0">
        <circle cx="300" cy="560" r="5"></circle><circle cx="470" cy="610" r="4"></circle><circle cx="640" cy="580" r="6"></circle>
        <circle cx="780" cy="630" r="4"></circle><circle cx="900" cy="560" r="5"></circle><circle cx="540" cy="650" r="3"></circle>
      </g>
    </svg>
  </div>
  <div id="__bundler_loading">Unpacking...</div>

  <script>
    
document.addEventListener('DOMContentLoaded', async function() {
  const loading = document.getElementById('__bundler_loading');
  function setStatus(msg) { if (loading) loading.textContent = msg; }

  // Error sink persists across replaceWith since it's on window, not the DOM.
  window.addEventListener('error', function(e) {
    var p = document.body || document.documentElement;
    var d = document.getElementById('__bundler_err') || p.appendChild(document.createElement('div'));
    d.id = '__bundler_err';
    d.style.cssText = 'position:fixed;bottom:12px;left:12px;right:12px;font:12px/1.4 ui-monospace,monospace;background:#2a1215;color:#ff8a80;padding:10px 14px;border-radius:8px;border:1px solid #5c2b2e;z-index:99999;white-space:pre-wrap;max-height:40vh;overflow:auto';
    d.textContent = (d.textContent ? d.textContent + String.fromCharCode(10) : '') +
      '[bundle] ' + (e.message || e.type) +
      (e.filename ? ' (' + e.filename.slice(0, 60) + ':' + e.lineno + ')' : '');
  }, true);

  try {
    const manifestEl = document.querySelector('script[type="__bundler/manifest"]');
    const templateEl = document.querySelector('script[type="__bundler/template"]');
    if (!manifestEl || !templateEl) {
      setStatus('Error: missing bundle data');
      console.error('[bundler] Missing script tags — manifestEl:', !!manifestEl, 'templateEl:', !!templateEl);
      return;
    }

    const manifest = JSON.parse(manifestEl.textContent);
    let template = JSON.parse(templateEl.textContent);

    const uuids = Object.keys(manifest);
    setStatus('Unpacking ' + uuids.length + ' assets...');

    const blobUrls = {};
    await Promise.all(uuids.map(async (uuid) => {
      const entry = manifest[uuid];
      try {
        const binaryStr = atob(entry.data);
        const bytes = new Uint8Array(binaryStr.length);
        for (let i = 0; i < binaryStr.length; i++) bytes[i] = binaryStr.charCodeAt(i);

        let finalBytes = bytes;
        if (entry.compressed) {
          if (typeof DecompressionStream !== 'undefined') {
            const ds = new DecompressionStream('gzip');
            const writer = ds.writable.getWriter();
            const reader = ds.readable.getReader();
            writer.write(bytes);
            writer.close();
            const chunks = [];
            let totalLen = 0;
            while (true) {
              const { done, value } = await reader.read();
              if (done) break;
              chunks.push(value);
              totalLen += value.length;
            }
            finalBytes = new Uint8Array(totalLen);
            let offset = 0;
            for (const chunk of chunks) { finalBytes.set(chunk, offset); offset += chunk.length; }
          } else {
            console.warn('DecompressionStream not available, asset ' + uuid + ' may not render');
          }
        }

        blobUrls[uuid] = URL.createObjectURL(new Blob([finalBytes], { type: entry.mime }));
      } catch (err) {
        console.error('Failed to decode asset ' + uuid + ':', err);
        blobUrls[uuid] = URL.createObjectURL(new Blob([], { type: entry.mime }));
      }
    }));

    const extResEl = document.querySelector('script[type="__bundler/ext_resources"]');
    const extResources = extResEl ? JSON.parse(extResEl.textContent) : [];
    const resourceMap = {};
    for (const entry of extResources) {
      if (blobUrls[entry.uuid]) resourceMap[entry.id] = blobUrls[entry.uuid];
    }

    setStatus('Rendering...');
    for (const uuid of uuids) template = template.split(uuid).join(blobUrls[uuid]);

    // Strip integrity + crossorigin — blob URLs from a file:// document inherit
    // a null origin, so crossorigin forces a CORS fetch that SRI then rejects.
    // The manifest bytes are ours; SRI protects against CDN compromise, not this.
    template = template.replace(/\s+integrity="[^"]*"/gi, '').replace(/\s+crossorigin="[^"]*"/gi, '');

    const resourceScript = '<script>window.__resources = ' +
      JSON.stringify(resourceMap).split('</' + 'script>').join('<\\/' + 'script>') +
      ';</' + 'script>';
    // Inject after <head> so the DOCTYPE stays first; prepending the script
    // would push the parser into quirks mode. DOMParser always emits a <head>
    // (synthesizing one if the source HTML omitted it) but may carry
    // attributes through, so match the full opening tag. slice() rather than
    // replace() keeps us clear of $-pattern substitution in resourceScript.
    const headOpen = template.match(/<head[^>]*>/i);
    if (headOpen) {
      const i = headOpen.index + headOpen[0].length;
      template = template.slice(0, i) + resourceScript + template.slice(i);
    }

    // Parse the template and swap the root element. Scripts inserted via
    // DOMParser/replaceWith are inert per spec — re-create each with
    // createElement so they execute, awaiting onload for src scripts to
    // preserve ordering (React before ReactDOM before Babel before text/babel).
    const doc = new DOMParser().parseFromString(template, 'text/html');
    document.documentElement.replaceWith(doc.documentElement);
    const dead = Array.from(document.scripts);
    for (const old of dead) {
      const s = document.createElement('script');
      for (const a of old.attributes) s.setAttribute(a.name, a.value);
      s.textContent = old.textContent;
      // text/babel scripts with a src: fetch and inline. transformScriptTags
      // does XHR against the src, but blob:null/ from a file:// origin is
      // silently dropped. Inlining makes it a plain inline babel script,
      // which transformScriptTags handles unconditionally.
      if ((s.type === 'text/babel' || s.type === 'text/jsx') && s.src) {
        const r = await fetch(s.src);
        s.textContent = await r.text();
        s.removeAttribute('src');
      }
      const p = s.src ? new Promise(function(r) { s.onload = s.onerror = r; }) : null;
      old.replaceWith(s);
      if (p) await p;
    }
    // Babel standalone auto-transforms type=text/babel on DOMContentLoaded,
    // which fired before we swapped the document. Trigger manually if present.
    if (window.Babel && typeof window.Babel.transformScriptTags === 'function') {
      window.Babel.transformScriptTags();
    }
  } catch (err) {
    setStatus('Error unpacking: ' + err.message);
    console.error('Bundle unpack error:', err);
  }
});

  </script>

MIT License

Copyright (c) 2025-2026 Evan Howell (Fore-Wave)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

# The Planck Threshold — Visual Atlas

**An interactive, non‑linear field guide to temporal order at the Planck scale, the trembling of matter, and the rise of coherence from the very small to the world we can touch.**

> Part of the **MVRP / Fore‑Wave** open‑science program by Evan Howell.
> Companion to the Zenodo dataset *MVRP Framework: φ‑Geometry Effects on Physical Coherence* — **DOI [10.5281/zenodo.18167536](https://doi.org/10.5281/zenodo.18167536)**.

---

## What this is

A single, self‑contained HTML application — no install, no server, no build step. Open it and explore a **constellation map** of seven concept nodes through **three learning lenses**, then weave your own **connective tree** and record the epiphany it sparks.

It is a *map of an idea‑space*, not a claim of settled physics. Established results and contested/unverified ideas are clearly separated and flagged, in keeping with the MVRP tier ethos (Tier 1 proven · Tier 2 testable · Tier 3 speculation).

## Live

- **GitHub Pages:** `https://fore-wave.github.io/<repo-name>/` *(enable Pages → branch `main` → root, after you push this folder)*
- **Single file:** `index.html` works offline — download and double‑click.

## Features

- **Constellation map** — 7 nodes across 3 chapters; visited nodes glow and link up; progress persists locally.
- **Three lenses** — every node retells itself as **The Naturalist** (analogy & living systems), **The Visualist** (live diagrams), or **The Theorist** (key equations, lightly explained).
- **Live generative diagrams** — Planck‑threshold time‑foam, zitterbewegung tremble, a subharmonic time‑crystal lattice, the Kuramoto phase‑lock bridge, the topology→function lineage, and a phyllotactic spiral. All drawn in‑browser; no image assets.
- **The Connective Tree (Node 07)** — tap two concepts to grow or cut a link, trace the canonical path, and write an epiphany that saves to your device.
- **Tweaks panel** — brightness, cosmic intensity, starfield, motion, and four curated plasma palettes.

## The territory

**Chapters:** I. *The Floor of Time* → II. *The Trembling Seed* → III. *The Bridge to the World*.

**Concept nodes:** the Planck threshold · zitterbewegung · time crystals · jitter‑to‑macro scaling · topology→technology (a lineage of inquiry) · the same pattern in nature · the connective tree.

**Lineage of inquiry** (mapped, with evidential status flags — *not* endorsed as established fact): Tesla, Puthoff, Searl, Bedini, Bearden, Pais, Meyer.

## Run it locally

```bash
# Option A — just open the file
open index.html            # macOS    (or double-click)

# Option B — serve it (any static server)
python3 -m http.server 8080
# then visit http://localhost:8080
```

## How it's built

Plain HTML + CSS + React (via CDN) with the JSX compiled in‑browser. The published `index.html` here is a **fully inlined, offline build** — React, fonts, styles, and all logic are embedded in the one file. Source components (the un‑inlined versions) live in the project this was authored from.

## Citation

If you reference the Atlas or its parent dataset, please cite:

> Howell, E. (2025). *MVRP Framework: φ‑Geometry Effects on Physical Coherence — Comprehensive Dataset.* Zenodo. https://doi.org/10.5281/zenodo.18167536

A machine‑readable [`CITATION.cff`](./CITATION.cff) is included.

## Scientific references for the concepts visualised

These underpin the *established‑physics* layer of the Atlas (Tier 1–2):

- M. Planck (1900) — natural units defining the Planck scale.
- P. A. M. Dirac (1928), *Proc. R. Soc. Lond. A* **117**, 610 — the Dirac equation, from which zitterbewegung arises.
- E. Schrödinger (1930), *Sitzungsber. Preuss. Akad. Wiss.* — original analysis of *Zitterbewegung*.
- F. Wilczek (2012), *Phys. Rev. Lett.* **109**, 160401 — "Quantum Time Crystals."
- A. Shapere & F. Wilczek (2012), *Phys. Rev. Lett.* **109**, 160402 — "Classical Time Crystals."
- D. V. Else, B. Bauer & C. Nayak (2016), *Phys. Rev. Lett.* **117**, 090402 — Floquet (discrete) time crystals.
- Y. Kuramoto (1975) — coupled‑oscillator synchronization model.
- S. H. Strogatz (2000), *Physica D* **143**, 1 — "From Kuramoto to Crawford."
- S. Douady & Y. Couder (1992), *Phys. Rev. Lett.* **68**, 2098 — phyllotaxis & the golden angle as physical self‑organization.
- H. E. Puthoff (2002), *Found. Phys.* **32**, 927 — polarizable‑vacuum (PV) approach.

## Related Fore‑Wave projects

- **MVRP‑phi‑geometry‑framework** — the core dataset & protocols
- **phi‑finder** — φ patterns in LIGO/JWST/SETI/seismic data — live: https://phi-finder.netlify.app/
- **Phlossary (Phourth Edition)** — the indexed glossary
- **Time‑Crystal triad deep‑dive**

## License

- **Code:** MIT — see [`LICENSE`](./LICENSE)
- **Documentation & content:** CC‑BY‑4.0 (attribution to Evan Howell / Fore‑Wave)

## Acknowledgements

Authored by **Evan Howell** (Independent Researcher · [@EvanTheHowell](https://x.com/EvanTheHowell)). Visual atlas designed and engineered with Claude. The Atlas deliberately **excludes** the consciousness / "Q‑triad" material.

# Zenodo update text — paste into your next version's Description

*(Append this under your existing description. It announces the interactive Atlas
and supplies academic citations for the added conceptual material.)*

---

## NEW (Version 3.3) — Interactive Companion: *The Planck Threshold — Visual Atlas*

A self‑contained, browser‑based **visual learning tool** now accompanies this dataset. It maps,
in a non‑linear "choose‑your‑path" format, the conceptual thread running through the MVRP program:
**below the Planck scale, temporal order need not hold; from the trembling of the very small
(zitterbewegung), a time‑crystal‑like vibrational state can organise and climb, scale by scale,
into macroscopic coherence** — the same micro‑rhythm‑to‑macro‑form mechanism nature already uses.

**Access**
- Interactive tool (GitHub Pages): `https://fore-wave.github.io/<repo-name>/`
- Source & offline build: `https://github.com/Fore-Wave/<repo-name>`
- Single self‑contained file also attached to this record.

**What it contains**
- Seven concept nodes across three chapters, each presented through three learning lenses
  (analogy · live diagram · key equations).
- Live, generative diagrams (no image assets): Planck‑threshold time‑foam, zitterbewegung,
  a subharmonic time‑crystal lattice, Kuramoto phase‑locking (micro→macro), a topology→function
  lineage, and a phyllotactic (golden‑angle) spiral.
- A **Connective Tree** node where the reader links concepts and records their own synthesis.
- A lineage‑of‑inquiry node (Tesla, Puthoff, Searl, Bedini, Bearden, Pais, Meyer) presented
  **with evidential‑status flags** — mapped as a field of inquiry, not asserted as established result.

**Scope note.** The Atlas is a conceptual map. Established physics (Tier 1–2) is kept distinct
from contested/unverified ideas (flagged), consistent with this project's measurement‑only ethos.
The consciousness / "Q‑triad" material is intentionally **excluded** from this companion.

### Citations for the added conceptual material

- M. Planck (1900) — natural units defining the Planck scale.
- P. A. M. Dirac (1928), *Proc. R. Soc. Lond. A* **117**, 610–624 — the Dirac equation.
- E. Schrödinger (1930), *Sitzungsber. Preuss. Akad. Wiss.*, 418 — *Zitterbewegung*.
- F. Wilczek (2012), *Phys. Rev. Lett.* **109**, 160401 — "Quantum Time Crystals."
- A. Shapere & F. Wilczek (2012), *Phys. Rev. Lett.* **109**, 160402 — "Classical Time Crystals."
- D. V. Else, B. Bauer & C. Nayak (2016), *Phys. Rev. Lett.* **117**, 090402 — Floquet time crystals.
- Y. Kuramoto (1975) — coupled‑oscillator synchronization.
- S. H. Strogatz (2000), *Physica D* **143**, 1–20 — "From Kuramoto to Crawford."
- S. Douady & Y. Couder (1992), *Phys. Rev. Lett.* **68**, 2098–2101 — phyllotaxis & the golden angle.
- H. E. Puthoff (2002), *Found. Phys.* **32**, 927–943 — polarizable‑vacuum (PV) approach.


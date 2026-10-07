# Vertex Degree — Study Deck

An interactive, single-page study tool for learning **vertex degree**, the **handshake lemma**, and **degree sequences** in graph theory — built for Discrete Mathematical Structures (Module 5).

**Live demo:** https://claude.ai/artifact/DbqwhjC6GWSwZkXKV3DDc5

## What's in it

The page is organized into five sections, reachable from a sticky nav bar:

1. **Definitions** — eight core vocabulary cards: degree of a vertex, the handshake lemma, degree sequence, min/max degree (δ(G) / Δ(G)), regular graphs, isolated & pendant vertices, in-degree/out-degree for digraphs, and the odd-degree corollary.
2. **Worked examples** — three fully worked diagrams (a simple graph, a graph with a loop, and a regular graph K₄), each with the edge list, degree count, degree sequence, and a handshake check.
3. **Activities** — five guided, hands-on tasks that send you into the interactive tool (handshake pairing, building to a target degree sequence, finding regular graphs, trees & leaves, modeling a real network).
4. **Interactive tool** — a free-form graph builder on an SVG canvas:
   - **Add vertex** — click empty space to place one (minimum spacing enforced so vertices can't overlap)
   - **Add edge** — click two vertices to connect them; click the same pair again for a parallel edge; click one vertex twice for a loop (repeatable for multiple loops)
   - **Remove edge** — same gestures, in reverse
   - **Delete vertex** — removes a vertex and everything touching it
   - Presets: K₄, Cycle C₅, Star S₄, Path P₅, and a random graph
   - A live stats panel: vertex/edge count, Σdeg(v), the handshake check, δ(G)/Δ(G), regularity, full degree sequence, and a per-vertex table
   - A "quiz me" mode that asks for the degree of a random vertex on your current graph
5. **Exercises** — 8 questions answered inline with a stated input format for each. Submit all at once for a score out of 8, then **Try again** or **Show answers**.

## Running it

No build step, no dependencies. Just open `index.html` in any modern browser:

```bash
git clone <this-repo-url>
cd <repo-folder>
open index.html   # or double-click the file, or serve it with any static file server
```

## Tech

Plain HTML, CSS, and vanilla JavaScript — a single self-contained file. No frameworks, no package manager, nothing to install.

## Design

Dark "night sky" theme — vertices rendered as stars, edges as connecting lines — chosen to tie the subject matter to space/astronomy. Typefaces: Space Grotesk (headings/labels) and Inter (body text).

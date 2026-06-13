# ceu-public-thesis

Public-facing deliverables from my CEU MSc Business Analytics capstone with [ingatlan.com](https://ingatlan.com): **Budapest rental price prediction for listing upload**.

The full capstone lives in a private repository. Most project material — internal data, warehouse notebooks, model artifacts, the technical report, and client decision memos — is **NDA-bound** under the ingatlan.com engagement. This repository contains **copies** of the two deliverables written for public or general-audience release; the originals remain in the capstone repo.

## Contents

| Document | Path | What it covers |
| --- | --- | --- |
| **Public summary** (ETD) | [`public_summary/`](public_summary/) | A ~3-page CEU Electronic Theses and Dissertations summary for a general audience: product question, scope (Budapest rental flats, HUF/sqm target, MdAPE metric), artifact package overview, time-ordered validation design, cross-validation leaderboard (best result 9.84% MdAPE), feature and geospatial story, risks, and recommended next steps. Licensed CC BY 4.0. |
| **Final client presentation** | [`client_final_presentation_june2026.html`](client_final_presentation_june2026.html) | A self-contained HTML slide deck (~21 slides plus appendix) for the capstone defence and client readout: executive summary, decision scope, interim-to-final changes, artifact package, validation design, CV leaderboard, feature/SHAP story, geospatial enrichment, upload-flow UX recommendations, risks/mitigations, next steps, and discussion questions. Open in any browser; use arrow keys or on-screen controls to navigate. |

Together, these documents describe **what was built, how it was evaluated, and what was recommended** — without internal row-level data, proprietary field dictionaries, or the full technical report.

Some slides in the HTML deck embed maps and PNG charts from the capstone workspace. Those assets are not copied here; the narrative slides and inline charts still work, but map iframes and a few images will not load in this repository alone.

## Build / view

**Public summary** — requires LaTeX with `pdflatex`:

```bash
cd public_summary && make    # → main.pdf
```

**Presentation** — open the HTML file in a browser:

```bash
xdg-open client_final_presentation_june2026.html
```

## License

See [LICENSE](LICENSE) (CC0 1.0). The public summary text is additionally marked CC BY 4.0 in the document itself.

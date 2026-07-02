# ceu-public-thesis

Public-facing deliverables from my CEU MSc Business Analytics capstone with [ingatlan.com](https://ingatlan.com): **Budapest rental price prediction for listing upload**.

The full capstone lives in a private repository. Most project material — internal data, pipeline notebooks, model artifacts, the technical report, and client decision memos — is **NDA-bound** under the ingatlan.com engagement. This repository contains **copies** of the two deliverables written for public or general-audience release; the originals remain in the capstone repo.

## Contents

| Document | Path | What it covers |
| --- | --- | --- |
| **Public summary** (ETD) | [`public_summary/`](public_summary/) | A ~3-page CEU Electronic Theses and Dissertations summary for a general audience: product question, scope (Budapest rental flats, HUF/sqm target, MdAPE metric), artifact package overview, time-ordered validation design, cross-validation leaderboard (best result 9.84% MdAPE), feature and geospatial story, risks, and recommended next steps. Licensed CC BY 4.0. |
| **Final client presentation** | [`client_final_presentation_june2026.html`](client_final_presentation_june2026.html) | A self-contained HTML slide deck (24 slides) for the capstone defence and client readout: executive summary, decision scope, validation design, CV leaderboard, feature/SHAP story, public NDVI map, upload-flow UX recommendations, risks/mitigations, next steps, and appendix tables/charts. Open in any browser; use arrow keys or on-screen controls to navigate. |

Together, these documents describe **what was built, how it was evaluated, and what was recommended** — without internal row-level data, proprietary field dictionaries, listing-location maps, repository paths, or the full technical report.

### Presentation assets

Bundled under [`presentation_assets/`](presentation_assets/):

- `11_geo_ndvi_h3_r8_map.html` — Sentinel-2 NDVI greenness aggregated to H3 cells (public satellite context only)
- `20_best_model_shap_beeswarm.png`, `20_best_model_shap_group_importance.png`, `20_best_model_permutation_importance.png` — explainability charts

Maps that plotted individual listing locations (price, WorldPop/GHSL probes, NDVI anchor points) are **not** included in the public release.

## Build / view

**Public summary** — requires LaTeX with `pdflatex`:

```bash
cd public_summary && make    # → main.pdf
```

**Presentation** — open the HTML file in a browser (keep `presentation_assets/` alongside it):

```bash
xdg-open client_final_presentation_june2026.html
```

## License

See [LICENSE](LICENSE) (CC0 1.0). The public summary text is additionally marked CC BY 4.0 in the document itself.

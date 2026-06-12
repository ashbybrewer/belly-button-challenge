# Belly Button Biodiversity — Interactive D3 + Plotly Dashboard

**[▶ Live dashboard](https://ashbybrewer.github.io/belly-button-challenge/)**

An interactive dashboard exploring the Belly Button Biodiversity dataset — the microbial species (OTUs) found in 153 human navels. Pick a test subject; every panel re-renders.

## Panels
- **Top-10 OTU horizontal bar chart** for the selected subject
- **Bubble chart** of the full sample (OTU id vs abundance, sized and colored by population)
- **Demographic info card** (age, ethnicity, location, washing frequency)

All driven by `d3.json` reads of the bundled `samples.json`, with a dropdown change handler re-binding every chart — no page reloads, no server.

## Run it locally
Any static server works: `python -m http.server` → open `localhost:8000`.

**Skills:** D3 data loading, Plotly chart configuration, DOM manipulation, event-driven re-rendering.

*2026 revision note: repaired a broken script path (`static/js/app.js` was empty; the working code lived one directory up) and pointed all reads at the bundled dataset — the dashboard now runs anywhere, including GitHub Pages.*

---
*Built during the University of Texas Data Analysis Boot Camp (2023–24), with help from classmates, tutors, and AI tools — disclosed then, kept honest now.*

# World Cup Prediction

A static, single-page 2026 World Cup prediction dashboard. The page presents group-stage score predictions, live/result comparison fields, projected knockout paths, title probabilities, model-vs-market divergences, a backtest summary, and an interactive match-up simulator.

## Overview

The project is currently contained in `index.html` and runs directly in the browser. It does not require a build step, package manager, backend server, or database.

The dashboard includes:

- Tournament progress funnel from group stage to champion
- Predicted group standings and match scores
- Match-by-match cards with predicted, live, and final result states
- Knockout bracket projection
- Title probability chart based on Monte Carlo simulation output
- Model-vs-market disagreement highlights
- UCL knockout backtest summary
- Interactive "run your own" team-vs-team prediction tool
- Chinese/English language toggle

## How to Run

Open `index.html` in any modern browser.

No installation is required.

## Project Structure

```text
WorldCupPrediction/
├── index.html
└── README.md
```

## Data and Updates

This is a static page. Match data, real scores, live states, projections, and model outputs are embedded in `index.html`.

To update the dashboard, edit or regenerate the relevant data inside `index.html`, then reopen or refresh the page in the browser.

## Model Notes

The page describes an independent prediction model based on multiple observable team-strength dimensions. It compares model output against market expectations after the model scores are produced, rather than using betting odds as direct inputs.

The prediction engine shown in the page includes:

- Strength ratings by team
- Expected-goals conversion
- Poisson scoreline probabilities
- Monte Carlo tournament simulation output
- Historical backtest summary for model credibility

The results are intended for analysis and entertainment, not betting or financial advice.

## Browser Compatibility

The page uses standard HTML, CSS, SVG, and vanilla JavaScript. It should work in current versions of Chrome, Edge, Firefox, and Safari.

An internet connection may be needed for externally loaded Google Fonts. The core page content still renders without them.

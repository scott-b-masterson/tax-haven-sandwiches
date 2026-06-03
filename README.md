# STAX Lab Figure Submission

Editable source and export files for the STAX Lab AI figure-sharing submission.

## Files

- `index.html`: editable infographic source.
- `tax_haven_sandwiches_stax_lab_infographic.png`: PNG for upload.
- `assets/`: static panel images, including the rendered Pfizer network panel.
- `build_infographic_assets.py`: rebuilds the HTML and copies aggregate chart assets.
- `export_infographic.js`: renders the Pfizer network and exports the final PNG.

## Rebuild

From the project root:

```bash
/Users/scottmasterson/.cache/codex-runtimes/codex-primary-runtime/dependencies/python/bin/python3 stax_lab_figure_submission/build_infographic_assets.py
NODE_PATH=/Users/scottmasterson/.cache/codex-runtimes/codex-primary-runtime/dependencies/node/node_modules /Users/scottmasterson/.cache/codex-runtimes/codex-primary-runtime/dependencies/node/bin/node stax_lab_figure_submission/export_infographic.js
```

The export uses local aggregate figures and summary statistics only. No Orbis
microdata are included.

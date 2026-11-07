# Watervein benchmark reports

This repository publishes the benchmark reports generated locally for Watervein releases.

- Website: https://waterveinjs.github.io/benchmark/
- Source project: https://github.com/waterveinjs/watervein
- Benchmark implementation: https://github.com/waterveinjs/js-framework-benchmark

Each release report is preserved under `versions/<tag>/`. The latest release is linked from the home page.

## Publishing

The Watervein release command uploads a complete report archive to the matching GitHub Release, then dispatches `.github/workflows/publish.yml` with the release tag. The workflow extracts the report and deploys this repository to GitHub Pages.

Reports are measured on the release maintainer's local machine. GitHub-hosted Actions only publishes the already-generated files; it does not run the benchmark.

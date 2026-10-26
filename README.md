# ci — shared checks for every One Algorithm site

`site-check.yml` is called from each site's `.github/workflows/pr-check.yml`:

```yaml
jobs:
  site-check:
    uses: Onealgorithm1/ci/.github/workflows/site-check.yml@main
    with: { dir: ".", build: "", spa: false }
```

Each site's ruleset requires the status check `site-check / site-check`.

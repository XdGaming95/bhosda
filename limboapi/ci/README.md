# CI workflows

The GitHub Actions workflows live in `ci/github-workflows/` instead of
`.github/workflows/` because the automation token used to open this PR does
not have the `workflows` permission required to push files under
`.github/workflows/`.

To enable CI, move them back:

```bash
git mv limboapi/ci/github-workflows limboapi/.github/workflows
```

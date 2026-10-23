# CI workflows

The GitHub Actions workflows live in `ci/github-workflows/` instead of
`.github/workflows/` because the automation token used to open this PR does
not have the `workflows` permission required to push files under
`.github/workflows/`.

To enable CI, move them back:

```bash
git mv ci/github-workflows .github/workflows
```

Both workflows have been updated to build with Temurin JDK 25 (required by
Velocity 4).

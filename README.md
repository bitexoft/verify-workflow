# Bitexoft verification workflow

Reusable GitHub Actions workflow that verifies a delivery of a Bitexoft project in CI.
It holds nothing else: the platform and its content live elsewhere.

```yaml
jobs:
  verify:
    uses: bitexoft/verify-workflow/.github/workflows/verify.yml@v1
    with:
      delivery: A1
```

The workflow installs `bitexoft-verify` pinned to a version and runs
`bitexoft-verify check <delivery>`. Do not copy it: call it.

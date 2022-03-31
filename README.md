# Infra1

> This infra is compliant with version [1.0.0](https://github.com/example-policy-org/policy/releases/tag/1.0.0) of the company policy **only**

## Test policy locally

```bash
$ docker run --rm -ti -v $(pwd):/apps ghcr.io/example-policy-org/policy-checker

Checking policy version...
Policy version: 1.0.0
Fetching Policy...

Applying 1 policy to 1 resource...
(Total number of result count may vary as the policy is mutated by Kyverno. To check the mutated policy please try with log level 5)

Passed checks: 2, Failed checks: 0, Skipped checks: 0
```

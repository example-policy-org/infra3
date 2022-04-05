# Infra3

> This infra is compliant with version [2.0.1](https://github.com/example-policy-org/policy/releases/tag/2.0.1) of the company policy but its only using [1.0.0](https://github.com/example-policy-org/policy/releases/tag/1.0.0) and can be updated with a pull-request.


## Test policy locally

```bash
$ docker run --rm -ti -v $(pwd):/apps ghcr.io/example-policy-org/policy-checker

Checking policy version...
Policy version: 1.0.0
Fetching Policy...

Running policy checker...

       _               _
   ___| |__   ___  ___| | _______   __
  / __| '_ \ / _ \/ __| |/ / _ \ \ / /
 | (__| | | |  __/ (__|   < (_) \ V /
  \___|_| |_|\___|\___|_|\_\___/ \_/

By bridgecrew.io | version: 2.0.1034

terraform scan results:

Passed checks: 2, Failed checks: 0, Skipped checks: 0

Check: CUSTOM_AWS_1: "Check that all resources are tagged with the key - department"
	PASSED for resource: aws_s3_bucket.b
	File: /main.tf:1-6
Check: : ""
	PASSED for resource: aws_s3_bucket.b
	File: /main.tf:1-6
```

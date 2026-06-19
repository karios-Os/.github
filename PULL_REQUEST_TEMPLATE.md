<!--
Thank you for contributing to KariosOS!

Please go through the checklist below before requesting a review.
If your PR does not meet all requirements, please file it as a draft PR.
Core team members will only review your PR once all requirements are met
(unless the change is trivial, such as a typo fix).
-->

<!-- If your PR resolves an issue, please add it here. -->
Resolves #

## Description

<!-- A brief summary of what this PR does and why. -->

## Checklist

<!-- Please check off ALL items for every PR: -->

- [ ] I have read the [Contributing Guide](../CONTRIBUTING.md).
- [ ] Every commit in this PR includes a DCO `Signed-off-by` line (`git commit -s`).
- [ ] I have run existing tests locally and they pass.
- [ ] I have added tests for all new or changed behavior.

### Go checklist

<!-- If your PR contains Go code: -->

- [ ] I have run `golangci-lint` and receive no errors relevant to my code.
- [ ] I have only exported functions, variables, and structs that are intended for use from other packages.
- [ ] I have added meaningful comments to all exported functions, variables, and structs.

### Infrastructure / API checklist

<!-- If your PR changes API behavior or infrastructure logic: -->

- [ ] I have verified the change works against a live KariosOS node.
- [ ] I have updated API documentation if endpoints were added or changed.
- [ ] I have considered backward compatibility.

### Documentation checklist

<!-- If your PR changes documentation or the web interface: -->

- [ ] I have reviewed my changes in a local build.
- [ ] Screenshots are included where relevant.

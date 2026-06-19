# Contributing to KariosOS

First off, thank you for considering contributing to KariosOS! We believe that the best infrastructure software is built collaboratively by the engineers who actually use it.

We want to make contributing as frictionless as possible. To ensure that everyone retains ownership of their code and that the project remains legally healthy, we do not use a Contributor License Agreement (CLA).

Instead, we use the industry-standard Developer Certificate of Origin (DCO).

---

## The Developer Certificate of Origin (DCO)

The DCO is a lightweight way for contributors to certify that they wrote or otherwise have the right to submit the code they are contributing to the project. It was created by the Linux Foundation and is used by thousands of open-source projects.

Here is the full text of the DCO:

---

### Developer Certificate of Origin
**Version 1.1**

Copyright (C) 2004, 2006 The Linux Foundation and its contributors.

Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.

By making a contribution to this project, I certify that:

**(a)** The contribution was created in whole or in part by me and I have the right to submit it under the open source license indicated in the file; or

**(b)** The contribution is based upon previous work that, to the best of my knowledge, is covered under an appropriate open source license and I have the right under that license to submit that work with modifications, whether created in whole or in part by me, under the same open source license (unless I am permitted to submit under a different license), as indicated in the file; or

**(c)** The contribution was provided directly to me by some other person who certified (a), (b) or (c) and I have not modified it.

**(d)** I understand and agree that this project and the contribution are public and that a record of the contribution (including all personal information I submit with it, including my sign-off) is maintained indefinitely and may be redistributed consistent with this project or the open source license(s) involved.

---

## How to Sign Your Commits

You do not need to sign any legal documents to agree to the DCO. You simply add a `Signed-off-by` line to your git commit messages.

This line looks like this:

```
Signed-off-by: Jane Doe <jane.doe@example.com>
```

The easiest way to do this is to use the `-s` flag when committing:

```bash
git commit -s -m "Add incredibly fast new routing feature"
```

If you use a GUI client for Git, look for a checkbox that says "Sign-off commit" or "Add DCO sign-off".

### What if I forgot to sign my commit?

No problem! If your pull request is failing the DCO check, you can easily fix your local commit and push it back up.

**If it's just your last commit:**

```bash
git commit --amend --no-edit --signoff
git push origin <your-branch-name> --force-with-lease
```

**If you have multiple commits to fix:**

```bash
git rebase --signoff HEAD~X  # Replace X with the number of commits
git push origin <your-branch-name> --force-with-lease
```

---

## Setting Up Your Development Environment

_(Add instructions here on how to build the project locally, run tests, and spin up a development node.)_

---

## Pull Request Process

1. Ensure your code builds locally and all tests pass.
2. Ensure every commit in your PR includes a DCO `Signed-off-by` line.
3. Submit your PR and request a review from the core maintainers.

---

## Community

**Join the conversation** — come talk infrastructure, ask questions, share what you're building, and connect with other contributors.

- [Join our Discord](https://discord.gg/INVITE_LINK_HERE) — community discussions, Q&A, and announcements
- [GitHub Discussions](https://github.com/karios-os/karios-apis/discussions) — long-form technical discussions and RFCs
- [GitHub Issues](https://github.com/karios-os/karios-apis/issues) — bug reports and feature requests

If KariosOS has been useful to you, **starring the repo** is a great way to show your support and helps others discover the project.

---

## Security Vulnerabilities

Do not report security vulnerabilities through public GitHub Issues. See [SECURITY.md](../SECURITY.md) for the responsible disclosure process.

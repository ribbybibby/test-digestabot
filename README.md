# digestabot-examples

This repository contains examples of Github Actions workflows that extend the
functionality of `digestabot` for different use cases.

You can see the workflows in [`./.github/workflows`](.github/workflows).

The workflows create Pull Requests in this repository.

## Chainctl Image Diff

Runs `chainctl image diff` on the updates made by `digestabot`.

It includes a summary of the differences in the PR body.

It also avoids making changes that do not resolve any vulnerabilities. This
could prevent some of the toil of reviewing PRs for images that are frequently
updated.

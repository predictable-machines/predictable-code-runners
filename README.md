# Predictable Code Runners

Reusable GitHub Actions workflows for [Predictable Code](https://github.com/predictable-machines/predictable-code).

## Usage

This repository contains reusable workflows that are provisioned automatically by the Predictable Code GitHub App. You do not need to reference these workflows manually.

## Versioning

Workflows are pinned to major version tags (e.g., `@v1`). Compatible updates are applied automatically by moving the tag forward. Breaking changes introduce a new major version.

## Required Permissions

The caller workflow must grant these permissions for all features to work:

| Permission | Required by |
|------------|-------------|
| `contents: write` | Init branch creation and push |
| `pull-requests: write` | PR annotations |
| `security-events: write` | SARIF upload to GitHub Code Scanning |

## Current Workflows

| Workflow | Description | Tag |
|----------|-------------|-----|
| `proxy.yml` | Predictable Code verification, SARIF upload, and initialization | `@v1` |

# My Assistant Testing

A test repository for Claude Code GitHub Actions integration.

## Overview

This repository demonstrates the integration of Claude Code with GitHub Actions using 9Router as an API proxy layer.

## Features

- GitHub Issues integration with Claude Code
- Pull Request assistance
- Automated code review and implementation

## Setup

This repository uses 9Router as a proxy for the Anthropic API:

- 9Router runs on port `20128`
- Claude Code connects via `http://localhost:20128/v1`

## Usage

### Working with Issues

1. Create an issue or comment on an existing one
2. Tag `@claude` in your comment
3. Claude Code will analyze and respond to your request

### Working with Pull Requests

1. Open a pull request
2. Add a review or comment with `@claude`
3. Claude Code will review and provide feedback

## Workflow

The Claude Code workflow is defined in `.github/workflows/claude.yml` and handles:
- Issue comments
- PR reviews
- Code implementation tasks

## License

MIT

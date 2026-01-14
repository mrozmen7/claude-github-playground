# claude-github-playground

A test repository for experimenting with Claude Code's GitHub integration.

## What is this repo?

This is a playground repository where you can test how Claude Code interacts with GitHub issues and pull requests. It's set up with GitHub Actions that automatically trigger Claude when you mention `@claude` in issues or comments.

## How does it work?

This repository uses the [Claude Code GitHub Action](https://github.com/anthropics/claude-code-action) to enable AI-assisted development directly in GitHub. When you mention `@claude` in:

- Issue comments
- Pull request comments
- Issue descriptions
- Pull request reviews

Claude Code will automatically respond and can help with tasks like:

- Answering questions about code
- Implementing features
- Fixing bugs
- Writing documentation
- Reviewing code changes

## Getting Started

1. Create a new issue or pull request
2. Mention `@claude` in your comment or description
3. Ask Claude to help with something (e.g., "Please add a new feature" or "Can you explain this code?")
4. Watch as Claude analyzes the request and responds with a plan or implementation

## What's included?

This repository contains:

- **GitHub Actions workflows** (`.github/workflows/`) - Automated workflows that trigger Claude Code
  - `claude.yml` - Main workflow for issue and comment interactions
  - `claude-code-review.yml` - Automated code review workflow for pull requests

That's it! This is a minimal setup to demonstrate Claude Code's capabilities on GitHub.

## Learn More

- [Claude Code Action Documentation](https://github.com/anthropics/claude-code-action)
- [Claude Code CLI](https://code.claude.com)

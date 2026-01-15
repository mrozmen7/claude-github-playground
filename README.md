# claude-github-playground

A playground repository for learning and testing Claude Code GitHub integration.

## Purpose

This repository serves as a safe, hands-on learning environment for exploring how Claude Code interacts with GitHub. It's designed to help you:

- Understand how AI-assisted development works with GitHub
- Test Claude Code's capabilities in a controlled setting
- Learn best practices for AI-human collaboration in software development
- Experiment with automated workflows and branch management

Whether you're new to Claude Code or exploring its GitHub integration features, this playground provides a risk-free space to experiment and learn.

## The Development Workflow

This repository follows a structured workflow that mirrors professional software development practices:

### 1. Issue Creation
- A team member creates a GitHub issue describing a task, feature, or bug fix
- The issue should clearly describe what needs to be done

### 2. Branch Creation
- When `@claude` is mentioned in an issue or comment, Claude Code automatically creates a new feature branch
- Branch names follow the pattern: `claude/issue-{number}-{timestamp}`
- This keeps the main branch stable and allows for isolated development

### 3. Implementation
- Claude Code reads the repository rules from CLAUDE.md
- Makes the requested changes on the feature branch
- Follows coding standards and safety guidelines defined in the repository

### 4. Pull Request
- Claude Code commits changes with clear, descriptive commit messages
- Pushes the branch to GitHub
- Provides a link to create a Pull Request with a pre-filled description

### 5. Review
- Team members review the changes in the Pull Request
- Discuss any concerns or request modifications
- GitHub Actions automatically run tests and checks

### 6. Merge
- Once approved and all checks pass, the Pull Request is merged to main
- The feature branch can then be deleted
- Changes are now part of the main codebase

This workflow ensures all changes are:
- **Traceable**: Every change is linked to an issue
- **Reviewed**: No direct commits to main branch
- **Tested**: Automated checks run before merging
- **Documented**: Clear commit messages and PR descriptions

## The Role of CLAUDE.md

The [CLAUDE.md](./CLAUDE.md) file is a special configuration file that defines how Claude Code should behave in this repository. Think of it as a rulebook that Claude Code always follows.

**Key rules defined in CLAUDE.md:**

- **Branch Protection**: Always create a new branch; never push directly to main
- **Commit Standards**: Use clear, descriptive commit messages
- **PR Requirements**: Open a Pull Request for every change
- **Safety Guidelines**: Never expose secrets, ask before destructive operations
- **Communication Style**: Use simple explanations and step-by-step approaches
- **Definition of Done**: Criteria for considering a task complete

By having these rules in CLAUDE.md, the entire team (including Claude Code) works consistently and safely. It's like having a shared agreement on how development should happen.

## The Role of GitHub Actions

GitHub Actions automate quality checks and workflows in this repository:

- **Automated Testing**: Runs tests automatically on every pull request
- **Code Quality Checks**: Validates code standards and linting rules
- **Build Verification**: Ensures changes don't break the build
- **Status Reporting**: Shows green/red status badges on pull requests

These automated checks help catch issues early and ensure that only working, high-quality code gets merged to main. They work hand-in-hand with the manual review process to maintain repository health.

## Getting Started

Ready to try it out? Here's how:

1. **Create an Issue**: Open a new GitHub issue with a task description
2. **Invoke Claude**: Mention `@claude` in the issue or a comment
3. **Watch the Magic**: Claude Code will create a branch and make changes
4. **Review Changes**: Check the Pull Request that gets created
5. **Merge**: If everything looks good, merge the PR

## Learn More

- [Claude Code Documentation](https://claude.ai/code)
- [GitHub Actions Documentation](https://github.com/features/actions)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)

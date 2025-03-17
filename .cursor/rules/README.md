# Cursor Rules

Cursor Rules are documentation files that help Claude (the AI assistant in Cursor) better understand the codebase and follow project-specific guidelines.

## What Are Cursor Rules?

Cursor Rules act as specialized documentation that:

1. Provide context about project structure and conventions
2. Define workflow guidelines and best practices
3. Establish coding standards and patterns to follow
4. Help the AI make more informed suggestions

## How to Use Cursor Rules

- Rules are written in Markdown files with `.mdc` extension in this directory
- Each rule file should focus on a specific aspect of the project
- Claude will automatically reference these rules when relevant to your queries
- Rules help ensure consistent and project-compliant responses

## Current Rules

- **use-git.mdc**: Defines Git workflow practices, including branch naming, commit messages, and PR management

## Adding New Rules

To add new rules:

1. Create a new `.mdc` file in this directory
2. Follow a clear structure with headings and examples
3. Focus on one specific aspect of development
4. Provide concrete examples where applicable

Rules should be concise, specific, and actionable to be most effective. 
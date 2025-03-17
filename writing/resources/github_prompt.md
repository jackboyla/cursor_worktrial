# Stacked PR Workflow Instructions

## Setup

1. Install GitHub CLI: 
   - macOS: `brew install gh`
   - Windows: `winget install -e --id GitHub.cli`
   - Linux: `sudo apt install gh` or follow [installation guide](https://github.com/cli/cli#installation)

2. Authenticate GitHub CLI:
   ```
   gh auth login
   ```

## Phase 1: Planning

1. Create a TODO.md file with the following structure:
   ```
   # Project Implementation Plan
   
   ## Overview
   Brief description of the feature/project
   
   ## PR Structure
   Each task group will be implemented as a separate PR, building on previous PRs.
   
   ## PR 1: [Title]
   **Branch name**: `feature-name-part1`
   **Base branch**: `main` (or another target branch)
   **Complexity**: Low/Medium/High
   
   - [ ] Task 1
   - [ ] Task 2
   
   ## PR 2: [Title]
   **Branch name**: `feature-name-part2`
   **Base branch**: `feature-name-part1` (or another target branch)
   **Depends on**: PR 1
   **Complexity**: Low/Medium/High
   
   - [ ] Task 1
   - [ ] Task 2
   ```

2. Repeat the PR sections for each logical chunk of work
3. Keep each PR under 1000 lines of changed code when possible
4. Ensure each PR can be reviewed independently
5. Mark clear dependencies between PRs
6. Specify the base branch for each PR (what branch it should target)

## Phase 2: Implementation

For each PR in the TODO.md file:

### PR Creation

1. Create a branch based on appropriate base:

   ```
   # If based on main:
   git checkout main
   git checkout -b branch-name-from-todo
   
   # If based on another branch:
   git checkout target-branch-name
   git checkout -b branch-name-from-todo
   
   # If based on another PR:
   gh pr checkout <base-pr-number>
   git checkout -b branch-name-from-todo
   ```

2. Implement all tasks for the PR
3. Write tests and documentation as needed

### Committing Changes

1. Format commit messages with:
   ```
   git commit -m "(PR #<number>): <Brief description>
   
   - <Detail of what changed>
   - <Another detail>
   
   Made with [cursor.sh](https://cursor.sh)"
   ```

2. Push changes and create PR with specific target branch:
   ```
   git push -u origin branch-name-from-todo
   
   # For PRs targeting main (default):
   gh pr create --title "PR #<number>: <Title from TODO.md>" --body "Implements tasks from TODO.md PR #<number>"
   
   # For PRs targeting a specific branch:
   gh pr create --base target-branch-name --title "PR #<number>: <Title from TODO.md>" --body "Implements tasks from TODO.md PR #<number>"
   ```

3. If PR depends on another PR:
   ```
   gh pr comment <pr-number> --body "Depends on #<dependent-pr-number>"
   ```

## Phase 3: Review and Iteration

1. Address review comments for each PR
2. Rebase as needed to maintain clean history
3. Update the TODO.md with status changes
4. Do not proceed to next PR until current one is approved

## Example Commit Message
```
(PR #2): Implement user authentication

- Added login form component
- Created authentication service
- Added unit tests for auth flow

Made with [cursor.sh](https://cursor.sh)
``` 
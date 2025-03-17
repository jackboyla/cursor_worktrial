# Teaching Vibe Coder GitHub Workflow

Date Started: 2023-06-15
Status: Idea

## Overview

A methodology for teaching LLM-based coding assistants (like Vibe Coder) to effectively use GitHub and structure work into reviewable chunks through automated TODO.md creation and stacked PR organization.

## Key Points

- LLMs need guidance on Git/GitHub best practices
- TODO.md as a standard first step in any coding project
- Structuring work into logically grouped, reviewable PRs
- Improving code review quality and efficiency

## AIDA Framework

- **Attention**: "Most LLM coding assistants produce code but struggle with professional Git workflows, leading to messy repositories and difficult code reviews."
- **Interest**: "By implementing a standardized TODO.md + stacked PR approach, LLMs can organize work in a way that mirrors best practices of senior developers."
- **Desire**: "Imagine having your AI assistant automatically break down complex tasks into perfectly organized, reviewable chunks that make collaboration seamless."
- **Action**: "Implement this workflow template in your LLM prompts to transform how you collaborate with AI coding assistants."

## Value Equation (Hormozi)

Dream Outcome × Perceived Likelihood of Achievement ÷ Time Delay ÷ Effort & Sacrifice = Value

- **Dream Outcome**: Perfect organization of code changes with minimal human intervention, leading to better code quality and team efficiency
- **Likelihood**: High - relies on structured prompting patterns that LLMs excel at following
- **Time**: Immediate implementation with progressive improvements as the LLM learns the pattern
- **Effort**: Low - requires only adding standardized prompts to your workflow

## Features vs. Benefits Analysis

| Feature | Benefit |
|---------|---------|
| Automatic TODO.md generation | Creates clear roadmap for implementation and ensures nothing is missed |
| Stacked PR organization | Makes code review manageable and focused on specific functionality |
| Standardized workflow | Reduces cognitive load when switching between human and AI collaboration |
| GitHub best practices | Ensures repository history remains clean and professional |

*Remember: Features tell, benefits sell. Features are facts about your product/idea, while benefits explain why those facts matter to the reader.*

## Notes

Research needed on optimal PR sizing and grouping strategies. Consider developing standard prompts that can be reused across projects. Could potentially be expanded into a VS Code extension or GitHub action to automate parts of the workflow.

## To-Do

- [ ] Document the exact prompting pattern for TODO.md generation
- [ ] Create examples of well-structured TODO.md files for different project types
- [ ] Define guidelines for optimal PR sizing and grouping
- [ ] Test the workflow on real projects and measure improvement in review efficiency

## Timeline

- [ ] First draft: 2023-07-01
- [ ] Revisions: 2023-07-15
- [ ] Final version: 2023-07-30 
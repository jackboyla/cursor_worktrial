---
title: "Best Practices for AI-Assisted Development Workflows"
author: "Jason Liu"
date: "2025-03-17"
---

# Best Practices for AI-Assisted Development Workflows

Imagine this: you open Cursor, request a new feature in YOLO-mode, and watch it start working. You flip back to Slack, reply to a few messages, check email, and then come back...

It's still running.

What the fuck is happening? `.sh` files are popping up. You glance at the source control tab—there's a Makefile, a random new `.gitignore`. Anxiety creeps in. Should you interrupt it? Could you break something important?

But wait—version control has been around since 1972. GitHub, after all, is designed exactly for reviewing and managing unexpected changes. Open-source communities have handled complex patches for decades.

> "Cursor, make a `todo.md` and break up these changes into multiple commits and pull requests."

```bash
brew install gh
gh auth login
```

Done.

## A core subnarrative 

The AI narrative in software development is misleading. When Devin came out, headlines claim "AI Replaces Developers"—like when Deep Blue beat Kasparov, or AlphaGo defeated Lee Sedol.

But look what happened: chess and Go players didn't vanish—they adapted. Grandmasters use engines to prepare, analyze, and teach. Coaches use engine analysis in lessons. Go professionals study AI games to find new strategies.

The software parallel is direct. Chess engines became core tools for pros and students alike. AI coding assistants will become fundamental to how we build and learn software. This isn't about replacement—it's about mastering a new approach.

Cursor's stance: We build tools for both pros and students to work and learn. Whether you're an engineer using AI to speed up work, or a student learning with AI guidance, we're here. The future isn't "AI instead of developers"—it's developers using AI as a tool, just as chess masters use engines today. Coding is just a small slice of what it means to build software. 

## Two Audiences, One Opportunity

Cursor can capture two kinds of builders,  after conversations with Aman and Michael, it's clear our core users are professional developers who collaborate within teams. And in particular strong network effects arise when Cursor integrates into these collaborative workflows.


## We should be educating developers at all levels

AI-assisted development doesn't replace coding fundamentals—it reinforces them:

- **Version Control**
- **Code Review**

Like chess players evolving from fearing engines to using them as training tools, developers are adapting to AI assistance. Players went from 1600 to 2100 ELO by studying with engines - developers can level up the same way. Cursor should be guiding all developers through this transition, just as chess books shifted from teaching basic strategy to teaching engine-assisted analysis. We're not moving from human coding to AI coding agents -

Cursor shuold be defining AI-assisted development as its own discipline, with its own best practices and workflows. 

It should be the case that if you want to learn software development as a field, you should start with Cursor.

### Beginner Coders

Beginners benefit from structured, reversible workflows. Teaching new developers how to effectively use Git and Cursor together mitigates catastrophic errors:

- Small, incremental commits.
- Stackable pull requests for easy review.
- Clearly annotated PRs showing Cursor's role.

Beginners become confident, reducing hesitation and adopting best practices early on, its only going to help them be more productive as they enter the workforce. 

> From some conversations with other folks I think there is definitely a population of junior developers who don't want to use Cursor because it feels like they're going to be handicapped. 

### Professional Developers

Experienced developers want efficiency, readability, and faster reviews. Cursor helps by:

- Automatically breaking large PRs into logical, review-friendly commits.
- Reducing PR merge latency.
- Creating smaller, manageable PRs that senior developers prefer.

> From being like a fractional tech lead to a lot of other teams, I have pushed a lot of folks to have smaller pull requests and that's dramatically improved productivity. I've yet to teach them how they could use AI to make this a little bit better. But really my goal is to have them adopt these techniques so my life is easier as a reviewer. 

## Growth 

If you can come up with a couple of pieces of content in this direction, teaching about these workflows, then we have two things that we can leverage as organic growth. 

Embedding `.cursor/rules` in repositories or tagging PRs with "written by Cursor" acts as both quality assurance and growth strategy. These integrations:

- Increase passive visibility of Cursor's value.
- Drive organic growth through professional recommendations.

### Cursor Rules

A `.cursor/rules/readme.md` should explain Cursor rules to new users and demonstrate how they can encode best practices and workflows. This helps spread adoption while improving code quality, just needs to be mentioned passively in 'how to bake best practices into cursor`. 


### Aside: Commit and PR;

A simple Cursor rule in the 'use_git.mdc' could add a subtle signature to PRs, similar to Claude's approach. This provides passive visibility while remaining unobtrusive:

```
---
PR generated with [Cursor](cursor.sh)
```

## My thoughts:

The conversation has shifted from "human coding vs AI coding" to mastering AI-assisted development—a fundamentally different discipline. Cursor serves as both instructor and authority, enabling developers of all skill levels to excel through AI collaboration.

Just as chess and Go were transformed by AI, software development workflows are evolving rapidly. Cursor guides developers through this transformation, helping them not just keep pace but thrive in this new paradigm.

When demonstrating Cursor's capabilities, we should focus on a clear narrative:

Pain -> Feature -> Benefit -> Outcome

For example, with Git integration, we're not just showcasing version control features. We're demonstrating how Cursor makes life easier for:

- Beginners: Safer experimentation through organized commits and reversible changes
- Professionals: Faster PR reviews through AI-assisted commit organization and PR structuring

The outcome extends beyond "Cursor can use Git"—it enables concrete workflow improvements like:

- Faster PR review cycles
- More manageable code review processes
- Increased team productivity through better collaboration

-------

# Project Template

Date Started: 2025-03-17
Status: Draft

## Overview
`
A comprehensive guide on integrating AI tools like Cursor into development workflows, focusing on best practices for version control, code reviews, and team collaboration. This piece reframes the AI narrative from "replacement" to "augmentation," drawing parallels with how chess players adapted to computer engines.

## Key Points

- AI-assisted development requires new workflows and best practices, particularly around version control
- Both beginners and professionals benefit from structured Git workflows when using AI tools
- Drawing parallels between chess/Go AI adaptation and software development adaptation
- Cursor should position itself as both a tool and an educational platform for AI-assisted development

## AIDA Framework

- **Attention**: "Imagine this: you open Cursor, request a new feature in YOLO-mode, and watch it start working. You flip back to Slack, reply to a few messages, check email, and then come back..."
- **Interest**: The parallel between chess/Go players adapting to AI and developers adapting to AI coding assistants
- **Desire**: Concrete benefits like faster PR reviews, safer experimentation for beginners, and increased team productivity
- **Action**: Adopt AI-assisted workflows with proper version control practices; use Cursor as both a tool and guide

## Value Equation (Hormozi)

Dream Outcome × Perceived Likelihood of Achievement ÷ Time Delay ÷ Effort & Sacrifice = Value

- **Dream Outcome**: Developers becoming significantly more productive and confident with AI tools while maintaining best practices
- **Likelihood**: High, based on the demonstrated parallel with chess players who evolved from fearing engines to using them as training tools
- **Time**: Immediate benefits with proper version control integration; long-term skill development like chess ELO improvement
- **Effort**: Minimal, leveraging existing Git knowledge with new AI-assisted workflows

## Features vs. Benefits Analysis

| Feature | Benefit |
|---------|---------|
| Automatic PR organization | Faster review cycles and reduced merge latency |
| Integration with version control | Safer experimentation and reversible changes |
| AI-assisted commit structuring | More manageable, logical code review processes |
| .cursor/rules repository integration | Encoding of best practices and improved team collaboration |
| Educational content on AI workflows | Developers at all levels learn to effectively use AI tools |

## Notes

- Need to develop concrete examples of .cursor/rules implementations
- Consider creating a series of tutorials on Git + Cursor best practices
- Explore ways to measure improved productivity and review cycles

## To-Do

- [ ] Expand the beginner and professional sections with specific workflow examples
- [ ] Create sample .cursor/rules implementations
- [ ] Develop visual workflow diagrams for common scenarios
- [ ] Interview both junior and senior developers for actual case studies

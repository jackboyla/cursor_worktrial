---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# some information about your slides (markdown enabled)
title: "AI-Assisted Development Best Practices"
info: |
  ## AI-Assisted Development Workflows
  Best practices and strategies for working with AI coding assistants.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
---

# AI-Assisted Development Best Practices

We're entering a new era of software development where AI isn't replacing developers—it's transforming how we work. These best practices will help you navigate this shift successfully.

<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/cursor-ai" target="_blank" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
We're not moving from human coding to AI coding.
We're figuring out this new thing - AI-assisted development.

Just like chess players had to learn with engines, and Go players had to rethink territory after move 37...
-->

---
transition: fade-out
---

# The Challenge

The exhilaration of watching AI build features can quickly turn to anxiety when you lose track of what's happening:

```markdown
You ask an AI agent to build a feature. You check email, then return to your IDE...

it's. still. running.

What's happening? Why are there .sh files? Makefile? New .gitignore?
Should you interrupt it mid-file-write and risk breaking everything?
```

This is a common experience, but it doesn't have to be this way. The solution isn't to abandon AI assistance—it's to integrate it into proven development workflows.

<!--
This is a common experience for developers first working with AI agents.
The lack of control and understanding can be frightening.
But there are better ways to work with AI.
-->

---
layout: two-cols
---

# Core Principles

The foundation of successful AI-assisted development isn't about AI at all—it's about software engineering fundamentals.

Version control becomes your essential safety net when working with AI. It allows you to experiment freely while maintaining the ability to revert changes if needed.

AI should enhance your existing development practices, not replace them. By breaking large changes into smaller, manageable pieces, you maintain control while leveraging AI's capabilities.

::right::

# For All Developers

Regardless of experience level, certain practices are universally valuable:

Start with version control before involving AI in your workflow. Create small, focused commits that are easy to review and revert if necessary.

Document your AI interactions in commit messages to maintain a clear history. Use feature branches to isolate AI experiments from your main codebase.

Most importantly, review every change before committing—AI is your assistant, not your replacement.

<!--
The key insight is that we're not replacing traditional software development practices.
Instead, we're enhancing them with AI capabilities.
Version control was invented in 1972 for good reasons - those reasons still apply today.
-->

---
layout: image-right
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# The Chess Analogy

The evolution of chess provides a powerful parallel to what's happening in software development. When Garry Kasparov pioneered "Advanced Chess," he demonstrated that humans working with AI could outperform either humans or AI alone.

This collaborative approach led to entirely new strategies and ways of thinking about the game, while the fundamental rules remained unchanged.

In software development, we're experiencing a similar transformation. AI tools aren't replacing developers—they're creating a new paradigm where human creativity and AI capabilities combine to produce better results than either could achieve independently.

<!--
Just as chess players had to learn to play with engines,
developers need to learn how to work effectively with AI assistants.
-->

---
layout: two-cols
layoutClass: gap-16
---

# For Beginners

For those early in their development journey, AI assistance presents both opportunities and challenges. Your first IDE experience might include AI, but it's crucial to build good habits from the start.

Learning version control alongside AI tools helps establish a foundation of best practices. Understanding code patterns becomes easier with AI assistance, but you must develop the judgment to evaluate the code it generates.

Most importantly, proper workflows help beginners avoid catastrophic failures, building confidence while developing skills in a controlled environment.

::right::

# For Professionals

Experienced developers can leverage AI to transform team workflows. Code reviews become more efficient when AI-generated code follows consistent patterns and includes proper documentation.

Knowledge sharing improves as AI can explain code in accessible ways. Breaking complex features into stacked PRs becomes more manageable with AI assistance.

Teams that establish clear AI usage patterns see improved collaboration across different skill levels and projects, with natural growth of AI adoption through GitHub integrations and cross-team visibility.

<!--
Different audiences require different approaches,
but all benefit from well-structured AI assistance.
-->

---
layout: center
class: text-center
---

# The Version Control Safety Net

<div class="text-xl mb-4">
"Remember: version control was invented in 1972 for a reason."
</div>

Version control isn't just about tracking changes—it's about giving you the confidence to experiment with AI while maintaining control over your codebase.

<div class="grid grid-cols-2 gap-4 mt-8">
<div>

### Traditional Benefits
Version control has always helped us track changes, revert mistakes, review code, collaborate safely, and document history. These traditional benefits become even more critical when working with AI.

</div>
<div>

### AI-Enhanced Benefits
With AI assistance, version control evolves to support smaller, more focused commits with automatically generated messages. Complex features can be split into stacked PRs, making review processes more efficient while providing a safety net for AI experimentation.

</div>
</div>

<!--
Version control is our safety net when working with AI.
It allows us to experiment freely while maintaining control.
-->

---
layout: two-cols
---

# AI-Assisted Workflow

Successful AI collaboration follows a clear pattern:

1. **Create a new branch** specifically for your AI-assisted feature work, isolating changes from your main codebase.

2. **Use AI for small, logical chunks** of work rather than entire features at once, maintaining visibility into what's changing.

3. **Review and commit incrementally**, validating each piece before moving to the next and creating a clean history.

4. **Create human-friendly PRs** that are easy for teammates to review, with clear documentation of AI's role.

5. **Iterate based on feedback**, using AI to help address review comments and refine the implementation.

::right::

# Team Integration

For teams to succeed with AI, establishing shared practices is essential:

Create clear AI usage guidelines that define when and how AI should be used in your development process.

Implement `.cursor/rules` templates to standardize AI behavior across your codebase, ensuring consistent patterns.

Define PR review processes that account for AI-generated code, with appropriate tagging to provide context for reviewers.

Share successful patterns across teams to build institutional knowledge about effective AI collaboration techniques.

<!--
Success with AI requires both individual and team practices.
Start small, establish patterns, and scale what works.
-->

---
layout: image-right
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# Growth Strategies

AI adoption grows naturally when embedded in everyday workflows. Something as simple as tagging AI contributions creates awareness without disruption:

```markdown
PR generated with [Cursor](cursor.sh)
```

Successful organizations integrate AI through PR templates that include AI-specific guidance, team documentation explaining effective AI usage patterns, and educational content that helps developers at all levels understand best practices.

This organic approach builds visibility in open source projects and establishes your team as leaders in AI-assisted development, creating a virtuous cycle of adoption and improvement.

<!--
By embedding ourselves in workflows that impact others,
we can demonstrate value while spreading adoption naturally.
-->

---
layout: center
class: text-center
---

# Educational Opportunity

AI-assisted development represents a significant educational opportunity for the entire software industry.

<div class="grid grid-cols-2 gap-8">
<div>

### For Beginners
New developers benefit from learning best practices from day one, understanding code patterns through AI explanations, and building good habits with AI guidance. The right approach helps them avoid common pitfalls while accelerating their learning curve.

</div>
<div>

### For Professionals
Experienced developers can explore advanced AI workflows, implement team integration strategies, and optimize performance through AI assistance. Taking leadership in AI adoption positions them at the forefront of this industry transformation.

</div>
</div>

<!--
Education is key to successful AI adoption.
We need to teach both how to code and how to work with AI effectively.
-->

---
layout: center
class: text-center
---

# The Future of Development

We're witnessing a fundamental shift in how software is created. AI doesn't replace the fundamentals of good software development—it amplifies them, making well-established practices even more powerful.

<div class="text-xl text-gray-500 mt-4">
The formula is clear: Human + AI > Human or AI alone
</div>

By embracing this collaborative approach and establishing thoughtful workflows, we can harness AI's capabilities while maintaining the quality, reliability, and humanity that makes software valuable.

<div class="mt-12">

[Documentation](https://cursor.sh) · [GitHub](https://github.com/cursor-ai) · [Community](https://discord.gg/cursor)

</div>

<!--
The future of development is here.
Let's build it together, responsibly and effectively.
-->

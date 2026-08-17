# Benchmark and Gap Analysis

A review of the best existing Claude and AI courses, and what we should add or improve. Researched August 2026.

## What We Benchmarked Against

Anthropic's own platform (Anthropic Academy, on the Skilljar site) is the authoritative reference. We also reviewed the strongest paid and free courses elsewhere.

- Anthropic Academy: 17 courses across 5 tracks, all free, with shareable certificates. Key courses: Claude 101, Claude Platform 101, Building with the Claude API (84 lectures, 8 hours), Claude Code 101, Claude Code in Action, Introduction to Subagents, Introduction to Agent Skills, Introduction to MCP and MCP Advanced, and Introduction to Claude Cowork.
- Anthropic AI Fluency track: courses for educators, students, small businesses, and nonprofits, built on a shared framework and foundations.
- DeepLearning.AI with Anthropic: Claude Code (three concrete projects), Agent Skills, and Building toward Computer Use (multimodal prompting, prompt caching, tool use).
- Top Udemy courses: the Claude Code and Cowork Masterclass by Ryan Ahmed, AI Hero by Matt Pocock, and Frank Kane's Claude Code course.
- Coursera: IBM and Vanderbilt prompt engineering courses, plus Building with the Claude API.

## What The Best Courses Do That We Should Adopt

### 1. Claude Cowork, the desktop agent, is a major missing topic
Anthropic launched Cowork, a desktop agent that carries out multi step tasks in finance, legal, marketing, data analysis, and research. It appears across Anthropic Academy and the top Udemy course. We currently only mention computer control briefly. This deserves real coverage.

Action: expand Module 5 to give Cowork its own lessons, and reference it again in the industry module.

### 2. Anthropic's AI Fluency framework is a proven mindset spine
Anthropic teaches a shared framework built on four habits, often summarised as delegation, description, discernment, and diligence. It gives beginners a mental model for working with AI rather than just tips.

Action: introduce this framework in Module 1 as the mindset that runs through the whole course, and refer back to it in later modules.

### 3. Concrete, named capstone projects
DeepLearning.AI does not say build an app. It says build a retrieval chatbot, turn a data notebook into a dashboard, and build a web app from a design mockup. Named projects are more motivating and easier to follow.

Action: replace our generic capstones with three named projects per track, and add a short gallery of these up front so students know the destination.

### 4. Assessment and a certificate
Anthropic gives quizzes and a shareable certificate. This drives completion and gives students something to show employers.

Action: add a short graded assessment at the end, and issue a course certificate. Reinforce our per module reviews as real quizzes.

### 5. Evaluation of prompts and outputs
Production focused courses teach how to test and measure prompt quality, not just write prompts. We cover iteration but not measurement.

Action: add a short lesson in Module 3 on checking output quality and comparing prompt versions.

### 6. Multi agent systems as a stretch goal
Anthropic and the top courses go up to multi agent workflows. We introduce subagents but stop there.

Action: add a stretch lesson in Module 6 or 7 on coordinating several agents, kept optional.

### 7. Sector framing that matches learner identity
Anthropic splits fluency by identity: educator, student, small business, nonprofit. Our industry module is close, and we can name these groups directly so students see themselves.

Action: make sure the industry module explicitly names students, educators, small business owners, and nonprofits.

## What We Already Do Well, Confirmed By The Benchmark

- Covering all three surfaces, chat, Claude Code, and the API, in one journey. Anthropic teaches these as separate courses, so bringing them together is a genuine strength for beginners.
- The strong earning and freelancing focus, which the general market courses do not emphasise and which fits our audience.
- The single branching path so beginners and developers share a course without either group being left behind.
- Teaching current features such as Memory, Artifacts, Projects, Skills, connectors, and prompt caching.

## Where We Should Not Follow The Benchmark

- The enterprise deployment courses for Amazon Bedrock and Google Vertex AI are out of scope for our audience. A brief mention is enough.
- Anthropic's eight hour API course is deeper than our audience needs. Our three hour developer module is the right size for a general course.

## Summary Of Proposed Changes

1. Add real coverage of Claude Cowork, the desktop agent.
2. Introduce the AI Fluency framework as the mindset spine in Module 1.
3. Replace generic capstones with three named projects and show them early.
4. Add a final assessment and a course certificate.
5. Add a short lesson on evaluating prompt and output quality.
6. Add an optional multi agent stretch lesson.
7. Name learner identities directly in the industry module.

These changes keep the course at twenty hours. Cowork and the framework replace time from trimming the lightest existing lessons, so the total does not grow.

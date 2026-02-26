> **ALPHA**
> This is a new service. Your [feedback](https://github.com/defra/ai-dev-working-group/discussions) will help us improve it.

# DEFRA AI Dev Working Group

This repository is the central home for the DEFRA AI Dev Working Group. It exists to help DEFRA developers use AI coding tools well, starting with GitHub Copilot, through shared guidance, practical tutorials, tested prompts, and honest documentation of what works and what does not.

## About the working group

The DEFRA AI Dev Working Group started the way most useful things do: a small number of developers who were already using GitHub Copilot, had opinions about it, and wanted to compare notes. It was not set up by a programme board or handed down as an initiative. It grew because there was an obvious gap between what individual developers were discovering and what the wider DEFRA development community had access to.

The group is developer-led and open to any DEFRA developer who wants to be involved. There is no formal membership process. If you use GitHub Copilot, have something to contribute, or just want to follow along, you are welcome here.

### Mission

To help DEFRA developers get real, responsible value from GitHub Copilot by building a shared body of practical knowledge that reflects how we actually work.

That means being honest about limitations as well as strengths, keeping guidance grounded in DEFRA's technical context, and updating things when they go out of date rather than letting them drift.

### Goals

The working group has four broad goals that shape what we spend our time on.

The first is knowledge sharing. GitHub Copilot moves quickly. Features ship, behaviours change, and what worked well six months ago may not be the best approach today. The working group exists partly as a mechanism for DEFRA developers to share what they are learning with each other, rather than everyone having to work it out independently.

The second is feature evaluation. When GitHub releases something new, whether that is a new model, a new IDE capability, or an update to agent mode, the working group tests it in realistic DEFRA development contexts and documents what it actually does. The goal is to give developers an honest account of whether something is worth their time, not a summary of the release notes.

The third is ways of working. GitHub Copilot raises real questions about code review, about what responsible use looks like, and about how teams should handle AI-assisted output. The working group develops practical norms for these questions, informed by what teams are actually experiencing rather than what looks good on paper.

The fourth is influencing tooling strategy. Because the group sits close to day-to-day development work, it is well placed to inform decisions about AI tooling procurement, licensing, and policy within DEFRA. That is not the primary purpose of the group, but it is a useful consequence of the work.

## What you will find here

The repository is organised into the following sections.

**[Governance](/governance)** covers the guardrails for using GitHub Copilot within DEFRA. This includes what data you should not share with the model, how GitHub Copilot use sits within DEFRA's broader data handling policies, and how it aligns with Cabinet Office and NCSC guidance on AI tools in government. If you are unsure whether a particular use is appropriate, start here.

**[Playbooks](/playbooks)** contain practical guidance on integrating GitHub Copilot into your development workflow. This covers the AI-assisted software development lifecycle, how to set up your repository context to get more relevant suggestions, and what good code review looks like when AI-assisted code is involved.

**[Tutorials](/tutorials)** are step-by-step guides written by working group members. They cover getting started with GitHub Copilot in VS Code and JetBrains IDEs, using GitHub Copilot Chat effectively, working with pull request summaries, and using Agent Mode. Tutorials are reviewed before publishing and updated as GitHub releases new features.

**[Hints and Tips](/hints-and-tips)** is a lighter-weight, living collection of things the working group has found useful in day-to-day use. It is organised by feature area rather than workflow, and is intended to be browsed rather than read front to back.

**[New Features](/new-features)** tracks recently released GitHub Copilot features, records the working group's findings from testing them, and links to official GitHub documentation. The intent is to save you time when something new ships and you want to know whether it is worth exploring.

**[Prompt Library](/prompt-library)** holds a community-maintained collection of prompts that have been tested and found useful. Prompts are organised by task type and language. If you have a prompt that works well, the library is the right place to share it.

**[Ways of Working](/ways-of-working)** sets out the norms the working group has agreed on for using GitHub Copilot responsibly within teams. This includes how to approach AI-assisted commits, expectations in code review, and how to raise concerns or share learnings with the group.

**[Manager Guides](/manager-guides)** provides guidance for tech leads and delivery managers on licence and seat management, measuring adoption, and understanding how GitHub Copilot use is developing across their teams.

## Who this is for

This repository is for all DEFRA developers, regardless of experience level or how much you have used AI tooling before. Whether you are just getting started with GitHub Copilot, trying to get more out of it, or leading a team through adoption, there is something here for you.

## Quick start by role

If you are an engineer wanting to use GitHub Copilot effectively, the best starting point is the [Playbooks](/playbooks) section, followed by the [Tutorials](/tutorials) for your IDE. The [Governance](/governance) section is worth reading before you begin, particularly the guardrails document.

If you are a tech lead setting up your team, start with the context engineering guidance in [Playbooks](/playbooks), which covers how to structure your repository to get better results from GitHub Copilot. The [Ways of Working](/ways-of-working) section will help you establish team norms.

If you are a delivery manager or product owner, the [Manager Guides](/manager-guides) covers what you need to know about tooling, licences, and adoption. The [Governance](/governance) section provides the assurance context you may need for planning or reporting.

## Getting involved

Working group meetings are open to any DEFRA developer and are held regularly to review new GitHub Copilot features, share findings, and agree on content updates. You do not need to attend meetings to contribute, as pull requests and GitHub Discussions are equally valid ways to participate.

If you want to join, contribute content, or raise a question, you can do so through [GitHub Discussions](https://github.com/defra/ai-dev-working-group/discussions) or by opening a pull request directly. Before contributing content, please read [CONTRIBUTING.md](/CONTRIBUTING.md), which covers the content standards, review process, and how to submit changes.

## Staying current

GitHub releases GitHub Copilot updates frequently, and guidance can go out of date. Each document in this repository carries a review date. If you notice something that is no longer accurate, raising an issue or opening a pull request is the most useful thing you can do. You can watch this repository on GitHub to receive notifications when content is updated.

## Support and contact

For questions about this repository or the working group, raise a [GitHub Discussion](https://github.com/defra/ai-dev-working-group/discussions) or contact the working group via the DEFRA developer Slack channels.

## Licence

This repository is published under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/). You are welcome to reuse and adapt the content for your own government context. Where you do, please link back to this repository as the original source and share any improvements back via contribution.

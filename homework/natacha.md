# AI-Assisted Jira Ticket Creation - Learning Summary

## What I Wanted to Achieve

I wanted to use GitHub Copilot to create similarly structured, contextually rich, and very detailed Jira tickets.

The goal was to maintain consistency across multiple tickets while capturing the depth and nuance of each requirement.

### Tickets Created

- [SFD2-979](https://eaflood.atlassian.net/browse/SFD2-979)
- [SFD2-1003](https://eaflood.atlassian.net/browse/SFD2-1003)
- [SFD2-975](https://eaflood.atlassian.net/browse/SFD2-975)
- [SFD2-983](https://eaflood.atlassian.net/browse/SFD2-983)

---

## What I Did

I used a structured skill template for "Create a Jira Ticket from User Context" to guide the AI in generating comprehensive ticket specifications. 

I symlinked the skill to be able to access it in each repository I needed to use the context from.

The process involved:

1. **Initial Generation**: Provided the AI with architectural context, user requirements, and implementation scope
2. **AI Output**: Received well-structured tickets with title, description, acceptance criteria, and testing guides
3. **Collaborative Refinement**: Worked iteratively with the AI to improve ticket quality based on developer feedback

Because I wanted to be prompted for which model to use, it is likely I will find more refinements needed as each model seems to interpret instructions more or less as expected.

Not to name any names but `gpt-mini-5` did not create a markdown file by default and omitted a section, while ignoring my request for no labels. After trying to use this model a few times with refined skills, I decided it was not worth the inconvenience.

---

## How It Turned Out

### What Worked Well ✅

- **Consistent Structure**: The template ensured all tickets followed the same format, making them easier to triage and plan
- **Initial Quality**: First versions were impressive and contained good contextual understanding
- **AI Responsiveness**: The AI quickly adapted when I identified gaps and asked for improvements
- **Team Engagement**: Developer reviews prompted valuable feedback that led to ticket improvements
- **Can handed to agent to implement**: The context and plan are suitable to hand off to agent to do the work where code is involved

### Challenges Encountered ⚠️

- **Missing Technical Details**: The first versions lacked crucial details such as:
  - Expected input/output contracts
  - Specific API signatures or data structure examples
  - Validation rules and edge cases
- **Testing Guide Fitness**: The auto-generated testing guides were not fit for purposes—they were too generic and lacked the specificity needed for the testing team to execute effectively
- **Hallucinations**: One of the tickets had completely hallucinated requirements, I am not sure what I did wrong.
- **Hard to scope context when it spans across multiple repositories**: I manually copied a lot of markdown from other sources to offer the wider context. I guess this is maybe where MCP can help? I am not sure.

### Iteration and Improvement 🔄

Rather than accepting the initial output, I adopted a collaborative approach:

1. **Spot Issues Early**: I reviewed what was missing (input/output contracts, validation details) and explicitly asked the AI to incorporate these
2. **Developer Review Loop**: I had developers review the tickets, and their questions highlighted further gaps
3. **Targeted Fixes**: The most effective improvement was focusing on the testing guide—once I identified it as insufficient, I asked the AI to create specific, executable test scenarios with example payloads and expected outcomes
4. **Iterative Refinement**: Each iteration made the tickets more actionable and better aligned with what the implementation team actually needed

---

## Key Learnings

1. **AI Works Best with Feedback**: Don't expect perfect output on the first try. Treat the AI like a developer—review, critique, and iterate. The quality improvement from iteration was significant.

2. **Specificity Matters**: When asking the AI to add details, be specific about what's missing. Instead of "add more details," tell it "add input/output contract examples" or "include validation edge cases."

3. **Involve Your Team Early**: Developer feedback uncovered gaps I might have missed. Team involvement also builds confidence that the tickets are genuinely useful.

4. **Testing Guides Benefit Most from Real Constraints**: Generic testing guides are not helpful. When refining test scenarios, make sure the AI knows your actual environment, tools, and constraints (e.g., "we use curl for API testing" or "test data must be set up like this").

5. **Template Consistency is a Win**: Using a structured skill template meant all four tickets were consistent in format and depth. This made planning and handoff much smoother.

6. **Easy to miss AI mistakes**: Because I had given the agent so much context, and because of the time spent reviewing the tickets and iterating, I missed some glaring mistakes which led me to start working on non-sensical requirements. It's also a lot to review for human co-workers, the context and context of each ticket is rich and in a work environment with a lot of context switching, reviewing this is hard. 

---

## What I'd Do Differently Next Time

1. **More Upfront Context...if possible**: Provide the AI with example input/output contracts and validation rules at the start, rather than iterating to discover missing details
2. **Pre-Aligned Testing Strategy**: Before asking the AI to write the testing guide, clarify the testing environment, tools, and team constraints so it generates executable scenarios immediately
3. **Explicit Acceptance Criteria**: When defining acceptance criteria, ask the AI to include examples of valid and invalid inputs

---

## Bottom Line

Using AI to create detailed Jira tickets was helpful.

I think it will prove even more precious as time goes on and I refine the skill more and more to suit the needs of my team.

The initial output saved some time but also cost me some in the land of metacognition.
 
Refinement was needed, the collaborative iteration process actually improved ticket quality compared to if I'd written them manually.

I can also compare to my previous attempts (pre-AI) to use a template.
There was some consistency but often, the context was much poorer and the testing guide rougher around the edges.

The biggest value came from:

- Consistency across related tickets
- Quick turnaround on multiple complex specifications
- A capture of what's needed to change in the codebase which could be fed back directly to the AI agent

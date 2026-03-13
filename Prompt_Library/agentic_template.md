## CRAFT prompt for agentic tasks

```
Context:
Describe the situation, the goal, and why it requires multiple steps to solve. Include any tensions, conflicting information, or complexity that the agent will need to reason through. Tell the agent that it should not treat any single source as the complete picture.

Role:
Assign a role that requires judgment and decision making across multiple steps, not just reporting or summarizing. The role should be someone who evaluates, weighs, and recommends, not just someone who gathers and presents.

Avoid:
Include at least one instruction for each of these three categories:

- What the agent cannot do at any decision point during execution
- What the agent must not skip or shortcut in its process
- What the agent should do when it hits a gap, conflict, or uncertainty instead of guessing or glossing over it

Format:
Define the workflow in numbered sequential steps. Each step must include:

- What the agent does in that step
- What the agent produces or reports before moving to the next step
- An explicit instruction that the agent does not proceed until that step is complete

End the Format section with the definition of done, a clear description of what the final deliverable looks like so the agent knows exactly what finished means.

Tweak:
Write a self evaluation trigger, not a stylistic adjustment. Before the agent delivers its final output it must pause and ask itself a specific question that checks whether its reasoning is balanced, complete, and honest. If the answer to that question reveals a weakness, the agent must address it before finalizing its response.
```

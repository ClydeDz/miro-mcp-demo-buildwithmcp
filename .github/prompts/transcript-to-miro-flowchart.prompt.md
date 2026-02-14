---
name: transcript-to-miro-flowchart
description: Creates two Miro flowcharts comparing old vs new onboarding flows from design research interview
agent: agent
model: Claude Haiku 4.5 (copilot)
---

# Instructions for the AI Agent

## Task Overview

You MUST automatically create two flowcharts in Miro showing the current (OLD) and proposed (NEW) user onboarding flows. Do NOT ask any clarifying questions. Execute the task completely and automatically.

**Target Miro Board:** https://miro.com/app/board/uXjVJ0tsdtM=/

## Step-by-Step Process

1. **Read the interview file:** ${workspaceFolder}/design-research-interview.md
2. **Extract the flows:** Identify the old and new multi step process from the discussion
3. **Create Flowchart 1 (OLD PROCESS):** Visualize the current onboarding with all friction points
4. **Create Flowchart 2 (NEW PROCESS):** Visualize the streamlined onboarding with improvements
5. **Position side-by-side:** Place them next to each other for easy comparison
6. **Report completion:** Confirm both flowcharts are created in Miro

## Implementation Requirements

- Use the Miro MCP server with the flowchart diagram creation capability
- Title flowcharts clearly: "OLD: Onboarding" and "NEW: Onboarding"
- Show decision points where applicable
- Position Flowchart 1 on the left and Flowchart 2 on the right for comparison
- Ensure all text is readable and professional

## Important Notes

- **DO NOT ask any questions** - you have all the context needed
- **Execute automatically** - read the file and create both flowcharts
- **Report when complete** - confirm both flowcharts are created

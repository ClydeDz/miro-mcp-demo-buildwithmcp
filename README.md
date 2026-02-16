# Miro MCP Demo - Build With MCP - #MiroMCP

- [Competition post](https://www.reddit.com/r/miro/comments/1r25vm3/last_call_build_with_mcp_win_1000/)
- [Competition video submission](https://x.com/ClydeDz/status/2023410504753111181)

## Design research interview transcript
I've used Google Gemini to generate the transcript for a fictional design research interview. In a real world, this would be a recorded video which can be auto-transcribed using AI.

<details>
  <summary>Click to expand and view the prompt</summary>
  Create a transcript of a design research interview for me. Between an interviewer of a fictional bank called Bank of Goliath and an interviewee, here onward named as Candidate 1, who has signed up to this. 

The Bank of Goliath is wanting to improve their new customer onboarding experience and is conducting these design research interviews because of that. The interviewer is asking the Candidate 1 about what he thinks of the current onboarding process in details. Candidate 1 is very innovative and is an former finance guy experienced in this domain, and he explains cool ideas to uncomplicate the flow of the new customer onboarding experience where a new user can create their bank account in less than 10 minutes and in a mere 3 small steps compared to the old tedious approach of a 10 step workflow where the user had to provide so many details upfront and there was also backend logic that would direct the user into different conditional paths. The interviewer also explains the current process to the Candidate in details just so that the Candidate has a firm idea of what they're comparing with. 

As an AI agent, you are tasked to create a transcript of this interview from start to end. The interview lasts about 20 minutes. The transcript should contain, as mentioned above, the Candidate explaining how to make the process simpler, but the interviewer also explaining the current process. Intentionally, make the transcript non-linear, like a conversation that flows naturally, because there is someone else who is tasked with reading this transcript and coming up with a linear flow diagram of the old and new suggested process. This transcript should be this intentionally non-linear but should cover all the points above. 

If you can create a readme markdown file that would be great, otherwise something which I can easily copy paste.
</details>

- [Transcript 1 is for Project "Swift Goliath"](./design-research-interview.md)
- [Transcript 2 is for Project "Instant Zenith"](./design-research-interview-demo2.md)

In this example (this repo), the transcript markdown files are in the same project, so the AI Agent can get this as context.

## Miro MCP x VS Code 
I've set up Miro MCP server in VS Code IDE so I can chat with the AI Agent. While in Agent mode, I can ask it to read the interview transcript and generate a flowchart in Miro for me.

<details>
  <summary>Click to expand and view the prompt</summary>
  Hey AI agent, have a read thru the design-research-interview.md file attached in the context of this chat and create a flowchart in Miro using the configured Miro MCP server. I want to visualise what the candidate in this interview has suggested the new user onboarding flow could look like. 
</details>

## CoPilot prompt file
To automate further, we can use VS Code / CoPilot prompt file to provide all the instructions and context for the AI Agent to generate the flowchart using Miro MCP server.

The prompt file used in this video example can be [found here](./.github/prompts/transcript-to-miro-flowchart.prompt.md).












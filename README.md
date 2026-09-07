# AI Support Agent (n8n + Gemini)

An AI agent built in n8n that reads incoming customer messages, decides whether they're 
urgent, and if so, autonomously drafts a contextual reply — going beyond simple 
classification into actual decision-making and action-taking.

## How it works
1. A webhook receives an incoming customer message
2. An AI Agent (powered by Google Gemini) reads the message and reasons about it
3. If the message is urgent, the agent decides to call a custom tool that drafts 
   a personalized, empathetic reply
4. If not urgent, the agent simply notes "No action needed"
5. The result is sent back automatically

## How it's different from a basic AI workflow
Instead of following a fixed script (e.g. always outputting one word), the agent 
reasons about the situation and chooses whether to use a tool based on its own 
judgment — writing a unique, contextual response rather than a hardcoded one.

## Tools used
- n8n (AI Agent framework)
- Google Gemini API
- Python (for the custom draft_reply tool)

## Status
Fully functional — tested end-to-end with real webhook requests.

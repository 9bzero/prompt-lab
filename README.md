# prompt-lab

Test two system prompts side by side against the same input.

I kept copying prompts between tabs when iterating. Having both responses visible at the same time makes iteration much faster.

## Features

- Two-column layout: Prompt A vs Prompt B
- Shared user message sent to both simultaneously
- Each column has independent model, temperature, and max tokens
- Streaming responses in both columns
- Diff view: highlights where the responses diverge
- Save and load prompt pairs to localStorage

## Setup

```bash
npm install
cp .env.example .env
npm run dev
```

Works with any OpenAI-compatible API.

## Notes

Both calls fire in parallel — you're billed for both. Response time varies by model and load.

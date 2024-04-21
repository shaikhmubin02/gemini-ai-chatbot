<p align="center">
  An open-source AI chatbot app built with Next.js, the Vercel AI SDK, Google Gemini, and Vercel KV.
</p>

## Features

- Next.js App Router
- React Server Components (RSCs), Suspense, and Server Actions
- Vercel AI SDK for streaming chat UI
- Support for Google Gemini (default), OpenAI, Anthropic, Cohere, Hugging Face, or custom AI chat models and/or LangChain
- shadcn/ui
  - Styling with Tailwind CSS
  - Radix UI for headless component primitives
  - Icons from Phosphor Icons
- Chat History, rate limiting, and session storage with Vercel KV
- NextAuth.js for authentication

## Model Providers

Google Gemini `models/gemini-1.0-pro-001` as the default. However, thanks to the [Vercel AI SDK](https://sdk.vercel.ai/docs), you can switch LLM providers to [OpenAI](https://openai.com), [Anthropic](https://anthropic.com), [Cohere](https://cohere.com/), [Hugging Face](https://huggingface.co), or using [LangChain](https://js.langchain.com) with just a few lines of code.

## Running locally

> Note: You should not commit your `.env` file or it will expose secrets that will allow others to control access to your various Google Cloud and authentication provider accounts.

1. Install Vercel CLI: `npm i -g vercel`
2. Link local instance with Vercel and GitHub accounts (creates `.vercel` directory): `vercel link`
3. Download your environment variables: `vercel env pull`

```bash
pnpm install
pnpm dev
```

Your app should now be running on [localhost:3000](http://localhost:3000/).
# AI Math assistant Setup and Usage

## Overview
This guide will help you set up and run the AI Math assistant locally. The framework leverages self-healing tool-calling mechanisms to ensure accurate results.

---

## Prerequisites
Make sure you have the following installed:

- [Node.js](https://nodejs.org/) (latest version recommended)
- `npx` (comes with Node.js)

---

## Instructions

### 1. Create a .env File
Create a `.env` file in the root directory of your project and add your OpenAI and Langbase API keys. You can access your Langbase API key from [here](#).

Example `.env` file:

```
OPENAI_API_KEY=your_openai_api_key_here
LANGBASE_API_KEY=your_langbase_api_key_here
```

---

### 2. Start the BaseAI Server
To run the AI agent pipe locally, you need to start the BaseAI server. Use the following command in your terminal:

```bash
npx baseai@latest dev
```

---

### 3. Run the AI Agent Pipe
After starting the BaseAI server, execute the `index.ts` file to run the AI Agent Pipe. Use the following command:

```bash
npx tsx index.ts
```

---

### 4. Result
In your terminal, you’ll be prompted to:

```text
Enter your query:
```

For example, you can type:

```text
What is 120 cm in feet?
```

The AI agent will process the query. If the LLM produces an inaccurate result, the BaseAI framework’s self-healing mechanism will detect and correct the error, ensuring you receive the correct answer.

---

## Troubleshooting
If you encounter any issues:
1. Verify your Node.js version.
2. Check if `npx` and `tsx` are installed correctly.
3. Refer to the BaseAI documentation for advanced debugging.

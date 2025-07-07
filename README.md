# Skyscope Sentinel AI App Builder

![AI-Powered Full-Stack Web Development in the Browser](./public/social_preview_index.jpg)

Skyscope Sentinel AI App Builder developed by Miss Casey Jay Topojani allows you to choose the LLM that you use for each prompt from API or local Ollama AI model! Options include OpenAI, Anthropic, Ollama, OpenRouter, Gemini, LMStudio, Mistral, xAI, HuggingFace, DeepSeek, or Groq models - and it is easily extended to use any other model supported by the Vercel AI SDK! 



## Requested Additions

- ✅ OpenRouter Integration (@coleam00)
- ✅ Gemini Integration (@jonathands)
- ✅ Autogenerate Ollama models from what is downloaded (@yunatamos)
- ✅ Filter models by provider (@jasonm23)
- ✅ Download project as ZIP (@fabwaseem)
- ✅ Improvements to the main bolt.new prompt in `app\lib\.server\llm\prompts.ts` (@kofi-bhr)
- ✅ DeepSeek API Integration (@zenith110)
- ✅ Mistral API Integration (@ArulGandhi)
- ✅ "Open AI Like" API Integration (@ZerxZ)
- ✅ Ability to sync files (one way sync) to local folder (@muzafferkadir)
- ✅ Containerize the application with Docker for easy installation (@aaronbolton)
- ✅ Publish projects directly to GitHub (@goncaloalves)
- ✅ Ability to enter API keys in the UI (@ali00209)
- ✅ xAI Grok Beta Integration (@milutinke)
- ✅ LM Studio Integration (@karrot0)
- ✅ HuggingFace Integration (@ahsan3219)
- ✅ Bolt terminal to see the output of LLM run commands (@thecodacus)
- ✅ Streaming of code output (@thecodacus)
- ✅ Ability to revert code to earlier version (@wonderwhy-er)
- ✅ Chat history backup and restore functionality (@sidbetatester)
- ✅ Cohere Integration (@hasanraiyan)
- ✅ Dynamic model max token length (@hasanraiyan)
- ✅ Better prompt enhancing (@SujalXplores)
- ✅ Prompt caching (@SujalXplores)
- ✅ Load local projects into the app (@wonderwhy-er)
- ✅ Together Integration (@mouimet-infinisoft)
- ✅ Mobile friendly (@qwikode)
- ✅ Better prompt enhancing (@SujalXplores)
- ✅ Attach images to prompts (@atrokhym)(@stijnus)
- ✅ Added Git Clone button (@thecodacus)
- ✅ Git Import from url (@thecodacus)
- ✅ PromptLibrary to have different variations of prompts for different use cases (@thecodacus)
- ✅ Detect package.json and commands to auto install & run preview for folder and git import (@wonderwhy-er)
- ✅ Selection tool to target changes visually (@emcconnell)
- ✅ Detect terminal Errors and ask bolt to fix it (@thecodacus)
- ✅ Detect preview Errors and ask bolt to fix it (@wonderwhy-er)
- ✅ Add Starter Template Options (@thecodacus)
- ✅ Perplexity Integration (@meetpateltech)
- ✅ AWS Bedrock Integration (@kunjabijukchhe)
- ✅ Add a "Diff View" to see the changes (@toddyclipsgg)
- ⬜ **HIGH PRIORITY** - Prevent bolt from rewriting files as often (file locking and diffs)
- ⬜ **HIGH PRIORITY** - Better prompting for smaller LLMs (code window sometimes doesn't start)
- ⬜ **HIGH PRIORITY** - Run agents in the backend as opposed to a single model call
- ✅ Deploy directly to Netlify (@xKevIsDev)
- ✅ Supabase Integration (@xKevIsDev)
- ⬜ Have LLM plan the project in a MD file for better results/transparency
- ⬜ VSCode Integration with git-like confirmations
- ⬜ Upload documents for knowledge - UI design templates, a code base to reference coding style, etc.
- ✅ Voice prompting
- ⬜ Azure Open AI API Integration
- ⬜ Vertex AI Integration
- ⬜ Granite Integration
- ✅ Popout Window for Web Container(@stijnus)
- ✅ Ability to change Popout window size (@stijnus)

## Features

- **AI-powered full-stack web development** for **NodeJS based applications** directly in your browser.
- **Support for multiple LLMs** with an extensible architecture to integrate additional models.
- **Attach images to prompts** for better contextual understanding.
- **Integrated terminal** to view output of LLM-run commands.
- **Revert code to earlier versions** for easier debugging and quicker changes.
- **Download projects as ZIP** for easy portability Sync to a folder on the host.
- **Integration-ready Docker support** for a hassle-free setup.
- **Deploy** directly to **Netlify**


Get started now with the latest version of Skyscope Sentinel AI App Builder by pulling the repo!
```git clone https://github.com/skyscope-sentinel/Skyscope-AI-App-Builder```

- Next **click source.zip**

## Prerequisites

Before you begin, you'll need to install two important pieces of software:

### Install Node.js

Node.js is required to run the application.

1. Visit the [Node.js Download Page](https://nodejs.org/en/download/)
2. Download the "LTS" (Long Term Support) version for your operating system
3. Run the installer, accepting the default settings
4. Verify Node.js is properly installed:
   - **For Windows Users**:
     1. Press `Windows + R`
     2. Type "sysdm.cpl" and press Enter
     3. Go to "Advanced" tab → "Environment Variables"
     4. Check if `Node.js` appears in the "Path" variable
   - **For Mac/Linux Users**:
     1. Open Terminal
     2. Type this command:
        ```bash
        echo $PATH
        ```
     3. Look for `/usr/local/bin` in the output

## Running the Application

You have two options for running Skyscope Sentinel AI App Builder: directly on your machine or using Docker.

### Option 1: Direct Installation (Recommended for Beginners)

1. **Install Package Manager (pnpm)**:

   ```bash
   npm install -g pnpm
   ```

2. **Install Project Dependencies**:

   ```bash
   pnpm install
   ```

3. **Start the Application**:

   ```bash
   pnpm run dev
   ```
   
### Option 2: Using Docker

This option requires some familiarity with Docker but provides a more isolated environment.

#### Additional Prerequisite

- Install Docker: [Download Docker](https://www.docker.com/)

#### Steps:

1. **Build the Docker Image**:

   ```bash
   # Using npm script:
   npm run dockerbuild

   # OR using direct Docker command:
   docker build . --target skyscope-ai-app-builder
   ```

2. **Run the Container**:
   ```bash
   docker compose --profile development up
   ```

## Configuring API Keys and Providers

### Adding Your API Keys

Setting up your API keys in Skyscope Sentinel AI App Builder is straightforward:

1. Open the home page (main interface)
2. Select your desired provider from the dropdown menu
3. Click the pencil (edit) icon
4. Enter your API key in the secure input field


 **Note**: Custom base URLs are particularly useful when running local instances of AI models or using custom API endpoints.

### Supported Providers

- Ollama
- LM Studio
- OpenAILike

## Setup Using Git (For Developers only)

This method is recommended for developers who want to:

- Contribute to the project
- Stay updated with the latest changes
- Switch between different versions
- Create custom modifications

#### Prerequisites

1. Install Git: [Download Git](https://git-scm.com/downloads)

#### Initial Setup

1. **Clone the Repository**:

   
   ```git clone https://github.com/skyscope-sentinel/Skyscope-AI-App-Builder```

2. **Navigate to Project Directory**:

   ```bash
   cd Skyscope-AI-App-Builder
   ```

3. **Install Dependencies**:

   ```bash
   pnpm install
   ```

4. **Start the Development Server**:
   ```bash
   pnpm run dev
   ```

5. **(OPTIONAL)** Switch to the Main Branch if you want to use pre-release/testbranch:
   ```bash
   git checkout main
   pnpm install
   pnpm run dev
   ```
  Hint: Be aware that this can have beta-features and more likely got bugs than the stable release

>**Open the WebUI to test (Default: http://localhost:5173)**
>   - Beginngers: 
>     - Try to use a sophisticated Provider/Model like Anthropic with Claude Sonnet 3.x Models to get best results
>     - Explanation: The System Prompt currently implemented in Skyscope Sentinel AI App Builder cant cover the best performance for all providers and models out there. So it works better with some models, then other, even if the models itself are perfect for >programming
>     - Future: Planned is a Plugin/Extentions-Library so there can be different System Prompts for different Models, which will help to get better results

#### Staying Updated

To get the latest changes from the repository:

1. **Save Your Local Changes** (if any):

   ```bash
   git stash
   ```

2. **Pull Latest Updates**:

   ```bash
   git pull 
   ```

3. **Update Dependencies**:

   ```bash
   pnpm install
   ```

4. **Restore Your Local Changes** (if any):
   ```bash
   git stash pop
   ```

#### Troubleshooting Git Setup

If you encounter issues:

1. **Clean Installation**:

   ```bash
   # Remove node modules and lock files
   rm -rf node_modules pnpm-lock.yaml

   # Clear pnpm cache
   pnpm store prune

   # Reinstall dependencies
   pnpm install
   ```

2. **Reset Local Changes**:
   ```bash
   # Discard all local changes
   git reset --hard origin/main
   ```

Remember to always commit your local changes or stash them before pulling updates to avoid conflicts.

---

## Available Scripts

- **`pnpm run dev`**: Starts the development server.
- **`pnpm run build`**: Builds the project.
- **`pnpm run start`**: Runs the built application locally using Wrangler Pages.
- **`pnpm run preview`**: Builds and runs the production build locally.
- **`pnpm test`**: Runs the test suite using Vitest.
- **`pnpm run typecheck`**: Runs TypeScript type checking.
- **`pnpm run typegen`**: Generates TypeScript types using Wrangler.
- **`pnpm run deploy`**: Deploys the project to Cloudflare Pages.
- **`pnpm run lint:fix`**: Automatically fixes linting issues.

---


## FAQ

For answers to common questions, issues, and to see a list of recommended models, visit our [FAQ Page](FAQ.md).


# Licensing

MIT
Apache

# SpamGuard — Spam Detection Demo

## Project info

This is a self-developed demo project for detecting spam, phishing, and scam content using an AI gateway and Supabase for authentication and persistence.

## How can I edit this code?

You can edit and run this project locally or using your preferred cloud IDE.

### Edit locally

The only requirement is having Node.js & npm installed — we recommend using nvm if you manage multiple Node versions: https://github.com/nvm-sh/nvm#installing-and-updating

Follow these steps:

```sh
# Step 1: Clone the repository using the project's Git URL.
git clone <YOUR_GIT_URL>

# Step 2: Navigate to the project directory.
cd <YOUR_PROJECT_NAME>

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Start the development server with auto-reloading and an instant preview.
npm run dev
```

### Edit on GitHub

- Navigate to the desired file(s on GitHub.
- Click the "Edit" button (pencil icon) at the top right of the file view.
- Make your changes and commit.

### Use Codespaces or other cloud IDEs

You can also open the repository in GitHub Codespaces or your preferred cloud IDE and work there.

## What technologies are used for this project?

This project is built with:

- Vite
- TypeScript
- React
- shadcn-ui
- Tailwind CSS

## How can I deploy this project?

You can deploy this app using your preferred hosting provider (Vercel, Netlify, Supabase, etc.). If deploying serverless functions, ensure environment variables for your AI gateway and Supabase credentials are set in the target environment.

## Can I connect a custom domain to my project?

Yes — follow your hosting provider's instructions to connect a custom domain to your deployment.

---

## Environment variables

For local development create a `.env` file with your Supabase client values:

```
VITE_SUPABASE_URL="https://your-supabase-url"
VITE_SUPABASE_PUBLISHABLE_KEY="your-publishable-key"
```

When deploying the Edge Function (Supabase or other platform), ensure these server-side vars are set:

- `SUPABASE_URL`
- `SUPABASE_ANON_KEY`
- `AI_GATEWAY_URL` (e.g., https://api.your-ai-provider/v1/chat/completions)
- `AI_GATEWAY_API_KEY` (Bearer token for your AI provider)

These replace any provider-specific environment names referenced previously.

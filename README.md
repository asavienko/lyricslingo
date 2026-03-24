# LyricsLingo 🎵

Learn languages through songs. An interactive platform for language learning with AI-generated songs, lyrics with translations, and practice modes.

## Features

- 🎶 AI-generated songs for language learning
- 🌍 15+ languages supported
- 📚 Library of songs by genre, topic, and difficulty
- 🎯 Practice mode with vocabulary tracking
- 📊 Progress dashboard and achievements
- 🎧 Audio player with synced lyrics

## Tech Stack

- **Framework:** Next.js 16 + React 19
- **Styling:** Tailwind CSS v4 + shadcn/ui
- **Package Manager:** pnpm
- **Deployment:** Vercel

## Getting Started

```bash
# Install dependencies
pnpm install

# Run development server
pnpm dev

# Build for production
pnpm build
```

## Deployment

### 1. Create GitHub Repository

Push this code to a new GitHub repository:

```bash
git remote add origin https://github.com/YOUR_USERNAME/lyricslingo.git
git push -u origin main
```

### 2. Create Vercel Project

1. Go to [vercel.com](https://vercel.com) and sign in
2. Click "Add New Project"
3. Import your GitHub repository
4. Vercel will auto-detect Next.js settings

### 3. Configure GitHub Secrets (for CI/CD)

Get your Vercel credentials:

```bash
# Install Vercel CLI
npm i -g vercel

# Login
vercel login

# Link project (run in project directory)
vercel link

# Get project info
vercel project ls
cat .vercel/project.json
```

Add these secrets to your GitHub repository:
- `VERCEL_TOKEN` - from https://vercel.com/account/tokens
- `VERCEL_ORG_ID` - from `.vercel/project.json`
- `VERCEL_PROJECT_ID` - from `.vercel/project.json`

### 4. Deploy

Push to `main` for production deployment, or `develop` for preview.

## Project Structure

```
app/              # Next.js app routes
components/       # React components
  ui/             # shadcn/ui components
  dashboard/      # Dashboard-specific components
  library/        # Library view components
data/             # Static data (songs, blog posts)
hooks/            # Custom React hooks
lib/              # Utilities and API
public/           # Static assets
styles/           # Global styles
types/            # TypeScript types
```

## Environment Variables

None required for basic deployment.

---

Built with ❤️ for language learners everywhere.

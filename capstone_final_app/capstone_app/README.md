# 🎙️ Persona Call

An AI-powered speech-to-speech application that lets you have voice conversations with virtual personas of renowned software engineering experts.

![Next.js](https://img.shields.io/badge/Next.js-16-black?logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?logo=typescript)
![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)

## ✨ Features

- **Voice Conversations** – Real-time speech-to-speech interactions with AI expert personas
- **Expert Routing** – Intelligent system that matches your questions to the most relevant expert
- **Animated Portraits** – Dynamic video avatars generated using Gemini Veo
- **Visual Media Suggestions** – Contextual images and diagrams to reinforce concepts
- **Conversation Memory** – Persistent sessions stored in PostgreSQL

## 🛠️ Tech Stack

| Category | Technologies |
|----------|-------------|
| **Frontend** | Next.js 16, React 19, TypeScript, Tailwind CSS |
| **AI/ML** | OpenAI GPT, ElevenLabs TTS, Deepgram STT, Gemini Veo |
| **Database** | Vercel Postgres / Neon Serverless |
| **Storage** | Vercel Blob |
| **State** | Zustand |
| **Testing** | Vitest, Playwright |

## 📋 Prerequisites

- Node.js 18+
- npm or yarn
- API keys for:
  - OpenAI
  - ElevenLabs
  - Deepgram
  - Google Gemini (for video generation)

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone <repository-url>
cd capstone_app
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up environment variables

Create a `.env.local` file in the root directory:

```env
# OpenAI
OPENAI_API_KEY=your_openai_key

# ElevenLabs (Text-to-Speech)
ELEVENLABS_API_KEY=your_elevenlabs_key

# Deepgram (Speech-to-Text)
DEEPGRAM_API_KEY=your_deepgram_key

# Google Gemini (Video Generation)
GEMINI_API_KEY=your_gemini_key

# Database (Vercel Postgres or Neon)
POSTGRES_URL=your_postgres_url

# Vercel Blob Storage
BLOB_READ_WRITE_TOKEN=your_blob_token
```

### 4. Run the development server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 📁 Project Structure

```
src/
├── app/
│   ├── api/              # API routes
│   │   ├── call/         # Call session management
│   │   ├── expert/       # Expert routing
│   │   ├── speak/        # Text-to-speech
│   │   ├── transcribe/   # Speech-to-text
│   │   └── media/        # Media suggestions
│   └── page.tsx          # Main entry point
├── components/
│   ├── CallInterface.tsx     # Main call UI
│   ├── AnimatedPortrait.tsx  # Video avatar component
│   ├── ExpertBadge.tsx       # Expert info display
│   └── MessageBubble.tsx     # Chat message component
└── lib/
    ├── prompts.ts            # AI system prompts
    ├── router.ts             # Expert routing logic
    ├── persona-llm.ts        # LLM integration
    ├── elevenlabs.ts         # TTS integration
    ├── deepgram.ts           # STT integration
    └── persona-video.ts      # Video generation
```

## 🧪 Testing

```bash
# Unit tests
npm run test

# E2E tests
npm run test:e2e

# Test UI
npm run test:ui
```

## 🏗️ Build for Production

```bash
npm run build
npm start
```

## 📚 Additional Documentation

- [Animated Portrait System](./ANIMATED_PORTRAIT_README.md)
- [Media System](./MEDIA_SYSTEM_README.md)

## 👥 Team

*Capstone Project - 2024*

## 📄 License

This project is for educational purposes.

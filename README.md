<div align="center">
  <br />
    <img src="https://github.com/MadtorXD/podcastr/raw/main/public/icons/auth-logo.svg" alt="Podcastr Logo" width="200">
  <br />

  <div>
    <img src="https://img.shields.io/badge/-Typescript-black?style=for-the-badge&logoColor=white&logo=typescript&color=3178C6" alt="typescript" />
    <img src="https://img.shields.io/badge/-Next_._JS-black?style=for-the-badge&logoColor=white&logo=nextdotjs&color=000000" alt="nextdotjs" />
    <img src="https://img.shields.io/badge/-Tailwind_CSS-black?style=for-the-badge&logoColor=white&logo=tailwindcss&color=06B6D4" alt="tailwindcss" />
    <img src="https://img.shields.io/badge/-OpenAI-black?style=for-the-badge&logoColor=white&logo=openai&color=412991" alt="openai" />
    <img src="https://img.shields.io/badge/-Convex-black?style=for-the-badge&logoColor=white&logo=convex&color=222429" alt="convex" />
  </div>

  <h3 align="center">Podcastr — AI-Driven SaaS Podcast Platform</h3>

  <p align="center">
    Create, manage, and discover world-class podcasts with the power of Artificial Intelligence.
  </p>
</div>

---

## 📋 Table of Contents

1. 🤖 [Introduction](#introduction)
2. ⚙️ [Tech Stack](#tech-stack)
3. 🔋 [Features](#features)
4. 🤸 [Quick Start](#quick-start)
5. 🛡️ [Security & Authentication](#security)
6. 🚀 [Deployment](#deployment)
7. 📄 [License](#license)

## 🤖 Introduction

**Podcastr** is a premium AI-powered platform designed for the modern content creator. By integrating cutting-edge technologies like OpenAI's Text-to-Speech and DALL-E 3, Podcastr allows users to generate professional-grade audio content and striking visual thumbnails from simple text prompts. 

Whether you're an aspiring podcaster or a seasoned pro, Podcastr provides a unified dashboard to build, organize, and share your voice with the world.

## ⚙️ Tech Stack

- **Framework**: [Next.js 14 (App Router)](https://nextjs.org/)
- **Backend / Database**: [Convex](https://www.convex.dev/)
- **Authentication**: [Clerk](https://clerk.com/)
- **AI Engine**: [OpenAI (TTS & DALL-E 3)](https://openai.com/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **Components**: [Radix UI](https://www.radix-ui.com/) & [Shadcn UI](https://ui.shadcn.com/)
- **Animations**: [Framer Motion](https://www.framer.com/motion/)

## 🔋 Features

👉 **Robust Authentication**: A secure environment for creators with Clerk-powered login and registration.

👉 **AI Voice Generation**: Transform scripts into audio using multiple AI voices (Alloy, Echo, Fable, Onyx, Nova, Shimmer).

👉 **AI Thumbnail Studio**: Craft unique cover art using DALL-E 3 prompts directly within the app.

👉 **Dynamic Podcast Player**: A fixed, responsive player with full playback control (play/pause, seek, volume, Mute/Unmute).

👉 **Intelligent Discovery**: Search and filter through trending podcasts or explore by voice type and author.

👉 **Creator Profiles**: Dedicated spaces to showcase your work and track listener engagement.

👉 **Responsive Layout**: A sleek, dark-mode first interface optimized for desktops, tablets, and mobile devices.

## 🤸 Quick Start

To set up Podcastr locally, follow these steps:

### 1. Prerequisites

- [Git](https://git-scm.com/) installed.
- [Node.js](https://nodejs.org/) (Version 18 or higher recommended).
- [npm](https://www.npmjs.com/) or [pnpm](https://pnpm.io/).

### 2. Installation

```bash
# Clone the repository
git clone https://github.com/MadtorXD/podcastr.git

# Navigate to the directory
cd podcastr

# Install dependencies
npm install
```

### 3. Environment Setup

Create a `.env.local` file in the root directory:

```env
# Convex Configuration
CONVEX_DEPLOYMENT=
NEXT_PUBLIC_CONVEX_URL=

# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

# Clerk URLs
NEXT_PUBLIC_CLERK_SIGN_IN_URL='/sign-in'
NEXT_PUBLIC_CLERK_SIGN_UP_URL='/sign-up'

# OpenAI API
OPENAI_API_KEY=
```

### 4. Initialize the Backend

```bash
# Start the Convex development server
npx convex dev
```

### 5. Start the Application

```bash
npm run dev
```

Visit `http://localhost:3000` to start creating!

## 🛡️ Security & Authentication

Podcastr uses **Clerk** for session management and user protection. The **Middleware** is configured to protect all routes by default while allowing access to public sign-in and sign-up pages. 

The custom [middleware.ts](middleware.ts) ensures that static assets are served efficiently without unnecessary invocation, preventing system overhead.

## 🚀 Deployment

The project is optimized for deployment on [Vercel](https://vercel.com/). Ensure all environment variables are added to your Vercel project settings. For real-time user syncing, configure a **Clerk Webhook** pointing to your Convex HTTP endpoint (e.g., `https://<your-project>.convex.site/clerk`).

## 📄 License

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/) This project is licensed under the MIT License.

---

<div align="center">
  Built with ❤️ by <a href="https://github.com/MadtorXD">MadtorXD</a>
</div>

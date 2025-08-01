# 🤖 AI ChatPod - Your Personalized AI Chatbot Platform


[![Live Demo](https://img.shields.io/badge/Live%20Demo-ai--chatpod.vercel.app-blue)](https://ai-chatpod.vercel.app/edit-chatpod/25)
[![Next.js](https://img.shields.io/badge/Next.js-14-black)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-blue)](https://www.typescriptlang.org/)
[![Hasura](https://img.shields.io/badge/Hasura-GraphQL-purple)](https://hasura.io/)
[![Neon](https://img.shields.io/badge/Neon-PostgreSQL-green)](https://neon.tech/)

## 🚀 **The Future of Personalized AI Conversations**

Welcome to **AI ChatPod** - where cutting-edge AI meets seamless user experience! 🎯 This isn't just another chatbot; it's a **revolutionary platform** that allows you to create, customize, and deploy your very own AI-powered chatbots with the intelligence of **Google's Gemini AI**.

### 🌟 **What Makes AI ChatPod Extraordinary?**

- 🎨 **Fully Customizable Chatbots** - Create unique AI personalities for your business
- 🔐 **Secure Admin Dashboard** - Complete control over your chatbot fleet
- 💬 **Real-time Conversations** - Lightning-fast responses powered by Gemini AI
- 📊 **Session Management** - Track and review all chat interactions
- 🎯 **Guest-Friendly Interface** - No registration required for end users
- 🚀 **Production-Ready** - Deployed and scaled on Vercel

## 🏗️ **Tech Stack - The Dream Team**

| Technology | Purpose | Why We Chose It |
|------------|---------|-----------------|
| 🟢 **Next.js 14** | Frontend Framework | Server-side rendering, API routes, and incredible performance |
| 🔷 **TypeScript** | Type Safety | Because bugs are for debugging, not production |
| 🗃️ **Neon PostgreSQL** | Database | Serverless PostgreSQL that scales like magic |
| 🚀 **Hasura** | GraphQL API | Instant GraphQL APIs from PostgreSQL schema |
| 🤖 **Google Gemini AI** | AI Engine | State-of-the-art conversational AI |
| 🎨 **Shadcn/UI** | UI Components | Beautiful, accessible components out of the box |
| 🔐 **Clerk** | Authentication | Secure user management and session handling |
| ☁️ **Vercel** | Deployment | Zero-config deployment with global CDN |

## 📁 **Project Architecture - Organized Chaos**

```
bigprject2/ai-chatpod/
├── 🔧 Configuration Files
│   ├── .env.local                    # Environment secrets
│   ├── next.config.ts               # Next.js configuration
│   ├── tsconfig.json                # TypeScript config
│   ├── components.json              # Shadcn/UI config
│   └── package.json                 # Dependencies & scripts
│
├── 📱 Application Core
│   └── src/
│       ├── app/                     # Next.js App Router
│       │   ├── (admin)/             # 🔐 Admin Dashboard Routes
│       │   │   ├── edit-chatpod/    # Chatbot editing interface
│       │   │   └── review-session/  # Chat session analytics
│       │   ├── (guest)/             # 👥 Public Chat Interface
│       │   │   └── chatbot/[id]/    # Dynamic chatbot pages
│       │   └── api/                 # 🔌 API Routes
│       │       └── send-message/    # Real-time message handling
│       │
│       ├── components/              # 🧩 Reusable UI Components
│       │   ├── ui/                  # Shadcn/UI components
│       │   └── Messages.tsx         # Chat message renderer
│       │
│       └── lib/                     # 📚 Core Business Logic
│           ├── server/              # Server-side utilities
│           │   └── serverClient.ts  # Apollo GraphQL client
│           └── startNewChat.ts      # Chat initialization logic
│
├── 🗄️ Database & API Layer
│   ├── graphql/                     # GraphQL Schema & Operations
│   │   ├── queries/                 # Data fetching queries
│   │   ├── mutations/               # Data modification operations
│   │   └── apollo-client.ts         # Client-side GraphQL setup
│   │
│   ├── types/                       # 📝 TypeScript Definitions
│   │   └── types.ts                 # Shared type definitions
│   │
│   └── 🌱 Database Setup
│       ├── schema.graphql           # GraphQL schema definition
│       └── seed.sql                 # Initial data seeding
│
└── 🚀 Deployment & Build
    ├── .next/                       # Next.js build output
    ├── .vercel/                     # Vercel deployment config
    └── public/                      # Static assets
```

## 🚀 **Quick Start - Get Your ChatPod Running in Minutes!**

### Prerequisites
- Node.js 18+ 
- npm or yarn
- Neon PostgreSQL account
- Hasura Cloud account
- Google AI Studio account (for Gemini API)
- Clerk account

### 1. **Clone & Install**
```bash
git clone <your-repo>
cd bigprject2/ai-chatpod
npm install
```

### 2. **Environment Setup**
Create `.env.local` and add your secrets:
```env
# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_key
CLERK_SECRET_KEY=your_clerk_secret

# Hasura GraphQL Endpoint
NEXT_PUBLIC_HASURA_GRAPHQL_ENDPOINT=your_hasura_endpoint
HASURA_ADMIN_SECRET=your_hasura_secret

# Google Gemini AI
GEMINI_API_KEY=your_gemini_key

# Application URL
NEXT_PUBLIC_BASE_URL=http://localhost:3000
```

### 3. **Database Setup**
```bash
# Run the seed script to setup initial data
psql -h your-neon-host -d your-db -f seed.sql
```

### 4. **Launch Your ChatPod**
```bash
npm run dev
```

Visit `http://localhost:3000` and watch the magic happen! ✨

## 🎯 **Key Features - What Your Users Will Love**

### 👨‍💼 **Admin Dashboard**
- **Chatbot Management**: Create, edit, and configure multiple chatbots
- **Session Analytics**: Deep dive into conversation analytics
- **Real-time Monitoring**: Watch conversations happen in real-time
- **Custom Personalities**: Define unique AI personalities for different use cases

### 👥 **Guest Experience**
- **Zero Friction**: No registration required - just start chatting
- **Smart Conversations**: Powered by Google's Gemini AI
- **Persistent Sessions**: Conversations are saved and can be resumed
- **Beautiful UI**: Responsive design that works on all devices

### 🔧 **Technical Features**
- **Real-time Streaming**: Edge runtime for lightning-fast responses
- **GraphQL Integration**: Efficient data fetching with Hasura
- **Type Safety**: Full TypeScript coverage for bulletproof code
- **Scalable Architecture**: Built to handle thousands of concurrent chats

## 🌐 **Live Demo**

Experience AI ChatPod in action: [https://ai-chatpod.vercel.app/edit-chatpod/25](https://ai-chatpod.vercel.app/edit-chatpod/25)

## 🤝 **Contributing**

We welcome contributions! Whether it's:
- 🐛 Bug fixes
- ✨ New features
- 📚 Documentation improvements
- 🎨 UI/UX enhancements

## 🔮 **What's Next?**

- 📊 Advanced analytics dashboard
- 🔌 Webhook integrations
- 🎨 Custom theming options
- 📱 Mobile app
- 🌍 Multi-language support

## 📜 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Built with ❤️ by developers who believe AI should be accessible to everyone.**

*Ready to revolutionize your customer interactions? Deploy your own AI ChatPod today!* 🚀

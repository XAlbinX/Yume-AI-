<h1 align="center">🌙 Yume AI RP Chat Platform</h1>
<p align="center">
  <a href="https://yume-rp.vercel.app/"><b>LIVE DEMO</b></a> • 
  <b>Production-Ready AI SaaS</b> with Advanced Memory & Monetization
</p>

---

## ✨ Overview
Yume AI is a **full-stack AI chatbot platform** that blends:
- **Multi-model AI integration** (GPT-4, Claude, DeepSeek)
- **Persistent memory systems**
- **Stripe monetization**
- **Secure, scalable architecture**

Designed as a **portfolio-quality SaaS**, showcasing *end-to-end product development skills*.

---

## 🚀 Features

### 🧠 AI & Memory
- Dynamic model switching based on **credits & tier**
- Two-tier **conversation memory** with AI compression
- Context-optimized prompt engineering

### 💳 Monetization
- Dual-credit system (**daily free** + **premium persistent**)
- **Stripe subscriptions** + webhook automation
- Atomic, race-condition-safe transactions

### 🔒 Security & Auth
- Firebase Auth + Google OAuth
- Role-based permissions
- Secure file uploads & content moderation

### 📊 Real-Time Experience
- Live chat with typing indicators
- Message regeneration
- Real-time subscription & credit updates
- Optimized Firestore queries + caching

---

## 💻 Tech Stack

| Layer      | Tech |
|------------|------|
| **Frontend** | Next.js 14, React 18, TypeScript, Tailwind CSS |
| **Backend**  | Next.js API Routes, Firebase Functions |
| **Database** | Firebase Firestore (real-time) |
| **AI**       | OpenRouter API (multi-provider) |
| **Payments** | Stripe + Webhooks |
| **Storage**  | Firebase Storage |

---

## 🏗 Architecture Snapshot
```ts
// Smart model selection
const model = selectModel({
  credits: currentCredits,
  tier: getUserTier(userProfile),
  costPerMessage: CONFIG.CREDITS_PER_MESSAGE
});

// Safe credit deduction
await deductCredits(userId, creditCost);

// AI-powered conversation summary
await processConversationSummary(userId, botId, messages, getUserTier(userProfile));

```ts

📈 Key Points for Clients
✅ Idea → Production built solo
✅ Auth, payments, AI, analytics, storage in one app
✅ Fully mobile responsive
✅ Scalable & secure SaaS-ready foundation

📬 Let’s Talk
If you need AI-integrated SaaS or complex full-stack apps,
I can deliver production-grade quality fast.

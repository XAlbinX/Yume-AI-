<h1 align="center">🌙 Yume AI RP Chat Platform</h1>
<p align="center">
  <a href="https://yume-rp.vercel.app/"><b>LIVE DEMO</b></a> • 
  <b>AI SaaS Built to Solve Real Roleplay & AI Memory Challenges</b>
</p>

---

## ✨ Mission & Problem Solving
Yume AI was created with a clear mission:  
**To push the limits of AI roleplay platforms by solving industry pain points in immersion, memory, and cost-efficiency.**  

Most AI chat platforms today suffer from three major issues among others:

---

### **1️⃣ Poor Character Consistency & Shallow Roleplay**
**Problem:** Models drift from character personality, break immersion, or fail at long-form roleplay.  
**Solution:**  
- Selected **DeepSeek reasoning model** for superior contextual logic.  
- Applied **post-processing** to restructure responses for roleplay tone and format.  
- Designed **master-crafted roleplay prompts** to keep conversations authentic and reactive.

---

### **2️⃣ Short-Term Memory & Rising API Costs**
**Problem:** Most bots forget key plot points within 20–40 messages, and long context prompts drive API costs up fast.  
**Solution:**  
- Built a **two-tier memory system** that preserves essential plot, events, and character states for **200+ messages**.  
- Integrated **AI-powered compression** to retain accuracy while minimizing token usage.  
- Result: Extended continuity without the cost spiral.

---

### **3️⃣ No Real User Identity in Roleplay**
**Problem:** The AI rarely remembers *who the user is* in the roleplay, leading to generic responses.  
**Solution:**  
- Engineered **custom user persona injection** directly into prompts.  
- Every message keeps the AI aware of the user’s role, traits, and backstory for a richer narrative.

---

Yume AI is **not** a generic portfolio project — it’s an **R&D-driven SaaS** built in under **2 months of focused ~3h/day work** using GitHub Copilot for rapid iteration. Every feature exists to solve a real industry challenge.

---

### **Current challenge?**

Stripe/Paypal etc do not support AI chatbot platforms due to their NSFW potential. Currently exploring and developing multiple solutions for this to enable payments again.

---

## 🚀 Core Features

### 🧠 AI & Memory
- Multi-model AI switching (GPT-4, Claude, DeepSeek) based on **user tier & credits**  
- Two-tier **memory system** with AI compression for cost control  
- Context-optimized prompt engineering for consistent character portrayal  

### 💳 Monetization
- Dual-credit system (**daily free credits** + **persistent premium credits**)  
- Subscriptions + one-time pack purchases  
- Webhook automation with atomic, race-condition-safe transactions  

### 🔒 Security & Auth
- Firebase Auth + Google OAuth  
- Role-based access control  
- Content moderation & secure file handling  

### 📊 Real-Time Experience
- Live chat with typing indicators & message regeneration  
- Real-time subscription & credit sync  
- Optimized Firestore queries with caching for sub-100ms reads  

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
```

## 📈 Key Points for Clients
-✅ Built to solve real AI roleplay pain points, not just “demo tech”

-✅ Fully functional SaaS: auth, payments, AI, analytics, storage

-✅ Mobile-first, responsive, and production-ready

-✅ Scalable serverless architecture with enterprise-grade security

## 📬 Let’s Talk
If you need AI-integrated SaaS or complex full-stack applications with a clear product vision and technical depth,
I can deliver production-grade quality fast.

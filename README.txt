# SAVEIQ — Netlify Upload Version

Demo Link : 

Full Document : 

**SAVEIQ** is a smart financial goal tracker and planning application. This specific distribution is a standalone, fully client-side, **Netlify-ready version** optimized for instant, zero-config deployment. 

By eliminating complex backend dependencies, this build can be deployed in seconds via a simple drag-and-drop interface, making it perfect for rapid prototyping, staging environments, or private self-hosting.

---

## 🚀 Quick Start: Manual Deployment

Because this version is intentionally serverless and static, you can publish it online without installing any CLI tools or configuring environment variables.

1. **Prepare the Package:** Gather all files (ensuring `index.html` is at the root) into a single folder, or compress them into a `.zip` archive.
2. **Open Netlify:** Log in to your [Netlify Dashboard](https://netlify.com).
3. **Initiate Deploy:** Click on **Add new site** and select **Deploy manually**.
4. **Upload:** Drag and drop your folder or ZIP file into the designated upload zone.
5. **Go Live:** Netlify will instantly process your assets and provision a live SSL-secured URL (e.g., `https://netlify.app`).

---

## 🛠️ Architecture & Data Privacy

This lightweight version shifts all processing logic entirely to the client side, ensuring minimal overhead and high privacy compliance.

* **Local Persistence:** User accounts, financial profiles, and saving targets are safely isolated within the browser's native `localStorage`. Clearing browser data will reset the application state.
* **Deterministic AI Insights:** To eliminate the security risk of exposing private API tokens (such as Groq keys) in client-side code, AI-driven financial insights are generated using an intelligent browser-side rule engine. It evaluates your target parameters and maps them to tailored advisory outputs instantly.
* **Zero Network Overhead:** No external database queries, authentication handshakes, or server requests are required to run the core application loops.

---

## 📈 Roadmap: Scaling to Production

While this standalone package provides a seamless individual experience, transitioning to a scalable, multi-user production platform requires moving to the core **Source Version**. 

To upgrade to a persistent database model, you can leverage Netlify's ecosystem alongside external microservices:

| Feature | Local Upload Build (Current) | Production Source Build (Next Steps) |
| :--- | :--- | :--- |
| **Data Sync** | Isolated to a single device & browser | Cross-device syncing via an external DB (e.g., Supabase, MongoDB) |
| **Authentication** | Pseudo-accounts in `localStorage` | Secure JWT/OAuth identity management via Netlify Identity or Clerk |
| **AI Generation** | Client-side rule engine | Dynamic, live generative insights powered by secure **Netlify Functions** querying the Groq API |
| **Notifications** | Static in-app alerts | Real-time automated email delivery using transactional tools (e.g., Resend, SendGrid) |

---

## 📄 License & Terms

Distributed under the MIT License. See `LICENSE` for more information. Data collected by this static application never leaves your machine.

SAVEIQ — NETLIFY UPLOAD VERSION

This folder is a standalone Netlify-ready website.
To deploy manually:
1. Open Netlify.
2. Choose Add new site -> Deploy manually.
3. Upload this folder (or the ZIP containing this folder's contents).
4. Netlify will publish index.html.

This version is intentionally serverless/static so it can be deployed by drag-and-drop.
User accounts and goals are stored in browser localStorage. AI insights are generated from the goal data in the browser rather than exposing a Groq API key.

For production multi-user authentication, persistent database storage, real email delivery and Groq API access, deploy the source version through Netlify with Netlify Functions plus a hosted database/email provider.

# Help Me! — AI Student Assistant

A live, AI-powered student website with real chat built on Claude.

## Files in this project

```
index.html      ← The full website
api/chat.js     ← Serverless function (keeps your API key secret)
vercel.json     ← Deployment config for Vercel
README.md       ← This guide
```

---

## How to deploy on Vercel (Recommended — Free)

### Step 1 — Get your Anthropic API key
1. Go to https://console.anthropic.com
2. Sign up / log in
3. Click **API Keys** → **Create Key**
4. Copy the key (starts with `sk-ant-...`)

### Step 2 — Upload to GitHub
1. Go to https://github.com and sign up (free)
2. Click **New Repository** → name it `helpmeSite` → Create
3. Upload all 4 files (drag & drop the folder)

### Step 3 — Deploy on Vercel
1. Go to https://vercel.com → Sign up with GitHub (free)
2. Click **Add New Project** → Import your `helpmeSite` repo
3. Click **Deploy** (takes ~30 seconds)
4. Go to **Settings → Environment Variables**
5. Add:
   - Name: `ANTHROPIC_API_KEY`
   - Value: `sk-ant-...` (your key from Step 1)
6. Click **Redeploy** → your site is live!

### Your site URL will be:
`https://helpmeSite.vercel.app` (or similar)

Share this link with anyone — the AI chat will work for all visitors!

---

## How it works (for curious minds)

```
Visitor types a question
       ↓
index.html sends it to /api/chat
       ↓
api/chat.js (running on Vercel's servers) adds your secret API key
       ↓
Anthropic's Claude AI processes it
       ↓
Answer comes back to the visitor's screen
```

Your API key is NEVER visible to visitors — it stays safely on the server.

---

## Cost estimate
- Vercel hosting: **Free forever** (hobby plan)
- Anthropic API: ~**₹0.01–0.05 per message** (very cheap)
- 1000 student messages ≈ ₹10–50 total

---

## Need help?
Email: hello@reallygreatstudio.com

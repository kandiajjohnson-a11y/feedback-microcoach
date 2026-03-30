# Coach K's Feedback MicroCoach
**Kandid Conversations Global LLC**

An AI-powered coaching tool that helps leaders prepare difficult workplace conversations with clarity, care, and confidence.

---

## Deploy to Netlify (Step-by-Step)

### Step 1: Get Your Anthropic API Key
1. Go to **console.anthropic.com**
2. Sign up or log in (use a separate account from claude.ai)
3. Click **"API Keys"** in the left sidebar
4. Click **"Create Key"** — give it a name like "Feedback MicroCoach"
5. Copy the key immediately (it starts with `sk-ant-...`) — you won't see it again

### Step 2: Push to GitHub
1. Create a new repository on github.com (name it something like `feedback-microcoach`)
2. Upload all three files:
   - `index.html`
   - `netlify.toml`
   - `netlify/functions/chat.js`
3. Make sure the folder structure is exactly:
   ```
   index.html
   netlify.toml
   netlify/functions/chat.js
   ```

### Step 3: Connect to Netlify
1. Go to **app.netlify.com**
2. Click **"Add new site" → "Import an existing project"**
3. Connect to GitHub and select your repository
4. Build settings: leave everything blank (no build command needed)
5. Click **"Deploy site"**

### Step 4: Add Your API Key
1. In Netlify, go to **Site configuration → Environment variables**
2. Click **"Add a variable"**
3. Key: `ANTHROPIC_API_KEY`
4. Value: paste your key from Step 1
5. Click **Save**
6. Go to **Deploys → Trigger deploy → Deploy site** to restart with the new variable

### Step 5: Your tool is live!
Netlify will give you a URL like `https://your-site-name.netlify.app`
You can customize this under **Domain management**.

---

## File Structure
```
feedback-microcoach/
├── index.html                  # The full coaching interface
├── netlify.toml                # Netlify routing config
├── netlify/
│   └── functions/
│       └── chat.js             # Serverless function (holds API key securely)
└── README.md                   # This file
```

---

## Frameworks Built In
- Ask-Tell-Ask (high uncertainty situations)
- STAR Positive (celebrating success)
- STAR/AR Developmental (direct report / peer feedback)
- SBIR with Empathy (managing up)
- Conversation diffusers, 30-second rule, no-make-up rule
- Sensitive topic detection with extra care protocols
- Workload/prioritization language
- One-pager output with delivery reminders
- Follow-up email templates

---

*Built for Kandid Conversations Global LLC. All frameworks © Kandia / Coach K.*

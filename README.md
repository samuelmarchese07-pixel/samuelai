# Samuel AI — Trading Analysis Platform

App di analisi AI per trading su NAS100, S&P500 e XAUUSD.

## Stack
- Next.js 14 (App Router)
- Anthropic Claude (vision)
- Vercel (deploy)

---

## Deploy su Vercel (5 minuti)

### 1. Carica su GitHub
1. Vai su [github.com](https://github.com) → **New repository**
2. Nome: `samuel-ai` → Create
3. Carica tutti i file del progetto (drag & drop nella pagina del repo)

### 2. Collega a Vercel
1. Vai su [vercel.com](https://vercel.com) → Sign up con GitHub
2. **Add New Project** → seleziona `samuel-ai`
3. Clicca **Deploy** (Vercel riconosce Next.js automaticamente)

### 3. Aggiungi API Key
1. Nel progetto Vercel → **Settings** → **Environment Variables**
2. Aggiungi:
   - Name: `ANTHROPIC_API_KEY`
   - Value: la tua chiave da [console.anthropic.com](https://console.anthropic.com)
3. Clicca **Save** → poi **Deployments** → **Redeploy**

### 4. App live!
Vercel ti dà un URL tipo: `samuel-ai.vercel.app` 🚀

---

## Test locale
```bash
npm install
cp .env.example .env.local
# inserisci la tua API key in .env.local
npm run dev
# apri http://localhost:3000
```

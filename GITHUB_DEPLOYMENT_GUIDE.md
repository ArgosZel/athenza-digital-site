# GitHub Deployment Guide for Athenza Digital Site

## Quick Steps (5 minutes)

### 1. Create Repository
1. Go to https://github.com → Log in
2. Click **+ New repository** (green button, top‑right)
3. Name: `athenza-digital-site` (public)
4. ☑️ Initialize with README (optional)
5. Click **Create repository**

### 2. Generate Personal Access Token
1. Click profile icon → **Settings**
2. Left sidebar: **Developer settings** → **Personal access tokens** → **Tokens (classic)**
3. **Generate new token** → **Generate new token (classic)**
4. Fill:
   - Note: `Athenza-Static-Site-Deploy`
   - Expiration: 90 days (or "No expiration")
   - Scopes: ☑️ **repo** (full control)
5. **Generate token** → **COPY THE TOKEN IMMEDIATELY** (looks like `ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`)

### 3. Send Me These Three Things
1. **GitHub username** (e.g., `dimzel118562`)
2. **Repository name** (e.g., `athenza-digital-site`)
3. **Personal access token** (`ghp_xxxxxxxx...`)

## What Happens Next
1. I'll push the static site to your repo
2. Enable GitHub Pages in repo settings
3. Set up custom domain `athenzadigital.com`
4. Give you DNS records to update at Hostinger

## Alternative: Manual Upload (No Token)
1. Download `/home/argoszel/.openclaw/workspace/athenza-static-site.zip`
2. Go to your repo → **Add file** → **Upload files**
3. Drag & drop the unzipped `athenza-static-site` folder
4. Commit
5. Go to **Settings → Pages** → Source: `main` branch → `/ (root)` → **Save**

## DNS Update (After GitHub Pages is live)
Update Hostinger DNS with these A records:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

## Security Notes
- Token gives repo‑level access only (no admin)
- Revoke anytime under Settings → Developer settings → Personal access tokens
- Rotate after deployment if desired

---
**Time required:** ~15 minutes total hands‑on
**Cost:** $0/month (free GitHub Pages hosting)

*Guide generated: 2026-04-18 09:52 EET*
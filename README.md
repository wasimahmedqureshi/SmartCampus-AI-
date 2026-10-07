# 🎓 SmartCampus AI — Class 1–10 AI Learning Platform

An iStart Rajasthan Initiative · Bilingual (Hindi + English) · 100% Static (GitHub Pages Ready)

## 🚀 Deploy to GitHub Pages (5 minutes)

### Step 1: Firebase Setup
1. Open https://console.firebase.google.com → create project `smartcampus-ai`
2. Enable **Authentication** → Email/Password + Google
3. Enable **Firestore Database** (production mode, asia-south1)
4. Enable **Storage** (asia-south1)
5. Copy your web config → paste into `index.html` → `FIREBASE_CONFIG`

### Step 2: Firebase Rules
Firebase Console → Firestore → Rules → paste `firestore.rules` → Publish
Firebase Console → Storage → Rules → paste `storage.rules` → Publish
Firestore → Indexes → add indexes from `firestore.indexes.json`

### Step 3: Authorize GitHub Pages domain
Firebase Console → Authentication → Settings → Authorized domains →
add `<your-username>.github.io`

### Step 4: Push to GitHub
```bash
git init
git add .
git commit -m "SmartCampus AI MVP"
git branch -M main
git remote add origin https://github.com/<your-username>/smartcampus-ai.git
git push -u origin main

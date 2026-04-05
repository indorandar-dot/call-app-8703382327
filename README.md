# CallingApp — Vercel Deployment Guide

## Features (Advanced Version)
✅ Real-time messaging with **read receipts** (blue ticks)
✅ **Typing indicator** (animated dots)
✅ **Online/Offline status** with last seen
✅ **Message timestamps** + date dividers
✅ **Unread message badges**
✅ **Last message preview** in contact list
✅ **Contact info modal** with quick actions
✅ **Call timer** during calls
✅ **Mute / Camera toggle** during calls
✅ **Emoji picker** in chat
✅ **Contact search** bar
✅ **Toast notifications** (no ugly alerts)
✅ Beautiful redesigned UI

## Deploy to Vercel (3 Steps)

### Step 1 — Install Vercel CLI
```
npm install -g vercel
```

### Step 2 — Go to project folder
```
cd callingapp
```

### Step 3 — Deploy
```
vercel --prod
```

Vercel will give you a live URL like: `https://callingapp-xxx.vercel.app`

---

## Alternative: Drag & Drop on Vercel.com
1. Go to https://vercel.com/new
2. Click **"Import from Zip"** or drag the folder
3. Done!

## Firebase Rules (Recommended)
Set these in Firebase Console > Realtime Database > Rules:
```json
{
  "rules": {
    ".read": "auth != null",
    ".write": "auth != null"
  }
}
```

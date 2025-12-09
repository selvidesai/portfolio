# 🔐 Owner vs Visitor Guide

## How It Works Now

### ✅ **Password Protection Added!**

Your portfolio now has **password-protected uploads**. Here's how it works:

---

## 👤 **For You (Owner):**

1. **First Time Setup:**
   - Open `main.html` in your browser
   - Click "Choose Video" on any video card
   - Enter password: `portfolio2025` (change this in code!)
   - You're now in "Owner Mode" 🔒

2. **Uploading Videos:**
   - Click "Choose Video" button
   - Select video from your gallery/files
   - Video appears instantly
   - Edit title and description
   - Videos save automatically

3. **Owner Features:**
   - ✅ Upload videos
   - ✅ Edit titles/descriptions
   - ✅ See "Owner Mode" badge
   - ✅ Full control

---

## 👥 **For Visitors (Other Users):**

1. **What They See:**
   - Videos you uploaded (if using YouTube/Vimeo)
   - Read-only view (no upload buttons)
   - Can watch videos
   - Cannot upload or edit

2. **If They Try to Upload:**
   - Password prompt appears
   - They need your password to upload
   - Without password = no upload access

---

## ⚠️ **Important: Browser Storage Limitation**

### Current System (localStorage):
- Videos stored in **each browser separately**
- If you upload in Chrome → only Chrome sees it
- If visitor uploads → only their browser sees it
- **Videos don't share between users**

### Example:
```
You (Chrome): Upload Video 1 → Only you see it
Visitor (Firefox): Visits site → Doesn't see your video
Visitor uploads → Only visitor sees their video
```

---

## 🎯 **Solutions for Shared Videos**

### **Option 1: YouTube/Vimeo (Recommended for Portfolios)**
**Best for:** Showing same videos to everyone

**How:**
1. Upload videos to YouTube/Vimeo
2. Get embed links
3. Replace video code with iframe embeds
4. Everyone sees same videos

**Pros:**
- ✅ Everyone sees same videos
- ✅ No storage limits
- ✅ Fast loading
- ✅ Works everywhere

**Cons:**
- ❌ Videos are public on YouTube/Vimeo
- ❌ Need YouTube/Vimeo account

---

### **Option 2: Server/Backend**
**Best for:** Professional portfolio with custom hosting

**How:**
1. Host videos on server (AWS S3, Cloudinary, etc.)
2. Update code to load from server URLs
3. Everyone sees same videos

**Pros:**
- ✅ Full control
- ✅ Private videos possible
- ✅ Professional solution

**Cons:**
- ❌ Requires server/hosting
- ❌ More complex setup
- ❌ Costs money

---

### **Option 3: Current System (localStorage)**
**Best for:** Personal testing/development

**How:**
- Each browser stores videos separately
- Owner uploads → only owner sees
- Visitor uploads → only visitor sees

**Pros:**
- ✅ No server needed
- ✅ Free
- ✅ Easy setup

**Cons:**
- ❌ Videos don't share between users
- ❌ Limited storage (5-10MB per video)
- ❌ Cleared if browser cache cleared

---

## 🔧 **Change Your Password**

In `main.html`, find this line (around line 820):

```javascript
const OWNER_PASSWORD = "portfolio2025"; // Change this!
```

Change `"portfolio2025"` to your own secure password.

---

## 📝 **Quick Summary**

| User Type | Can Upload? | Can See Videos? | Storage Location |
|-----------|-------------|-----------------|------------------|
| **You (Owner)** | ✅ Yes (with password) | ✅ Yes | Your browser |
| **Visitor** | ❌ No (password required) | ⚠️ Only if using YouTube/Vimeo | Their browser (if they upload) |

---

## 🎬 **Recommended Setup for Portfolio**

For a professional portfolio where **everyone sees your videos**:

1. **Upload to YouTube/Vimeo:**
   - Create YouTube/Vimeo account
   - Upload your video edits
   - Make videos unlisted (not public) if you want privacy

2. **Get Embed Links:**
   - YouTube: Right-click video → Copy embed code
   - Vimeo: Share → Embed → Copy code

3. **Update Your HTML:**
   - Replace `<video>` tags with `<iframe>` embeds
   - Everyone will see your videos!

---

## ❓ **FAQ**

**Q: Can visitors upload videos?**
A: No, they need your password. Only you can upload.

**Q: Will visitors see videos I upload?**
A: Only if you use YouTube/Vimeo embeds. With localStorage, videos are browser-specific.

**Q: How do I make videos visible to everyone?**
A: Use YouTube/Vimeo embeds or host videos on a server.

**Q: Can I change the password?**
A: Yes! Edit `OWNER_PASSWORD` in the code.

**Q: What if I forget I'm in owner mode?**
A: Clear browser data or close browser. Next visit will ask for password again.

---

## 🚀 **Next Steps**

1. **Change password** in code (line ~820)
2. **Upload your videos** using owner access
3. **Decide:** Use YouTube/Vimeo for shared videos OR keep current system for personal use
4. **Test:** Open in different browser to see visitor view

---

**Need help?** Check the code comments or ask for assistance!








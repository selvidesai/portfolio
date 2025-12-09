# 📹 Video Upload Guide - Step by Step

## How Videos Are Stored in Browser

Your videos are stored in your browser's **localStorage** (a built-in browser storage). This means:
- ✅ Videos stay on your computer (not uploaded to internet)
- ✅ Videos persist when you refresh the page
- ✅ Works offline
- ⚠️ Videos are stored per browser (if you use Chrome, videos won't appear in Firefox)
- ⚠️ If you clear browser data, videos will be deleted

---

## 📱 How to Upload Videos - Step by Step

### **Step 1: Open Your Portfolio**
1. Find your `main.html` file in `e:\portfolio\`
2. Double-click `main.html` to open it in your browser
   - It will open in your default browser (Chrome, Edge, Firefox, etc.)

### **Step 2: Navigate to Video Section**
1. Scroll down to the **"Video reel"** section
2. You'll see 3 video cards with upload areas
3. Each card shows: 📹 icon and "Click to upload video from gallery"

### **Step 3: Upload Your First Video**
1. **Click** on the upload area (the box with 📹 icon) of the first video card
2. A file picker window will open
3. **Navigate** to where your videos are stored:
   - If videos are in **Photos/Gallery**: 
     - Windows: Go to `Pictures` folder or `This PC > Pictures`
     - Or search for your video file name
   - If videos are on your **phone**:
     - Connect phone to computer via USB
     - Or transfer videos to computer first
4. **Select** your video file (MP4, MOV, AVI, etc.)
5. Click **"Open"** or **"Select"**

### **Step 4: Video Appears Automatically**
- Your video will **instantly appear** in the video player
- The upload area will disappear
- Video is now stored in browser!

### **Step 5: Edit Title and Description**
1. Below the video, you'll see:
   - **Title box**: Change "Video 1" to your video name (e.g., "My Showreel 2025")
   - **Description box**: Add details about the video
2. Type your changes - they save automatically!

### **Step 6: Upload More Videos**
- Repeat Steps 3-5 for Video 2 and Video 3
- Each video card works independently

---

## 🎬 Visual Guide

```
┌─────────────────────────────────────┐
│  Video reel                         │
├─────────────────────────────────────┤
│                                     │
│  ┌──────────────┐  ┌──────────────┐│
│  │   📹         │  │   📹         ││
│  │ Click to     │  │ Click to     ││
│  │ upload...    │  │ upload...    ││
│  └──────────────┘  └──────────────┘│
│  [Video Title]     [Video Title]   │
│  [Description]     [Description]   │
└─────────────────────────────────────┘
         ↓ Click here
    [File Picker Opens]
         ↓ Select video
    [Video Appears!]
```

---

## 💾 How Browser Storage Works

### What Happens When You Upload:
1. **You select a video** → Browser reads the file
2. **Video is converted** → Converted to a format browser can store
3. **Stored in localStorage** → Saved in browser's storage
4. **Video URL created** → Browser creates a temporary link to play video

### Where It's Stored:
- **Location**: Browser's internal storage (not a folder you can see)
- **Access**: Only your browser can access it
- **Size Limit**: Usually 5-10MB per video (browser dependent)

---

## 🔄 Managing Your Videos

### To Replace a Video:
1. Click on the video player
2. Click the upload area again (it appears when you hover)
3. Select a new video

### To Delete a Video:
1. Open browser Developer Tools (Press `F12`)
2. Go to **Application** tab (Chrome) or **Storage** tab (Firefox)
3. Find **Local Storage** → your website URL
4. Delete items starting with `video-1`, `video-2`, `video-3`
5. Refresh the page

### To Clear All Videos:
1. Press `F12` to open Developer Tools
2. Right-click on the page → **Inspect**
3. Go to **Application** → **Local Storage**
4. Click **Clear All** or delete individual items
5. Refresh page

---

## ⚠️ Important Notes

### Browser Storage Limitations:
- **Size**: Each browser has limits (usually 5-10MB per video)
- **Total Storage**: Usually 5-50MB total per website
- **Persistence**: Cleared if you clear browser cache

### For Larger Videos:
If your videos are too large, consider:
1. **Compress videos** before uploading (use online tools like HandBrake)
2. **Upload to YouTube/Vimeo** and use embed links instead
3. **Host videos** on a server/cloud storage

---

## 🆘 Troubleshooting

### Video Not Uploading?
- ✅ Check file size (should be under 10MB)
- ✅ Check file format (MP4 works best)
- ✅ Try a different browser
- ✅ Clear browser cache and try again

### Video Not Showing?
- ✅ Refresh the page (F5)
- ✅ Check browser console for errors (F12)
- ✅ Try uploading a smaller video file

### Videos Disappeared?
- ✅ Check if you cleared browser data
- ✅ Videos are browser-specific (Chrome vs Firefox)
- ✅ Try uploading again

---

## 📝 Quick Checklist

- [ ] Open `main.html` in browser
- [ ] Scroll to "Video reel" section
- [ ] Click upload area (📹 icon)
- [ ] Select video from gallery/photos
- [ ] Video appears automatically
- [ ] Edit title and description
- [ ] Repeat for other videos
- [ ] Done! Videos are saved in browser

---

## 🎯 Summary

**Upload Process:**
1. Click upload area → 2. Select video → 3. Video appears → 4. Edit details → Done!

**Storage:**
- Videos saved in browser's localStorage
- Persist when you refresh page
- Stored locally on your computer
- No internet needed to view

**That's it!** Your videos are now part of your portfolio! 🎉








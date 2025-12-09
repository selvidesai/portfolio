# 📧 Email Setup Guide

## ✅ What's Fixed:

1. **"Let's connect" button** → Now opens Gmail (not Outlook)
2. **Contact form** → Now sends emails to selvidesai18@gmail.com

---

## 🚀 Quick Setup (5 minutes)

### **Option 1: EmailJS (Recommended - Automatic Email Sending)**

EmailJS is FREE and sends emails automatically without backend!

#### **Step 1: Create EmailJS Account**
1. Go to: https://www.emailjs.com/
2. Click **"Sign Up"** (free account)
3. Sign up with your Gmail: **selvidesai18@gmail.com**

#### **Step 2: Create Email Service**
1. After login, go to **"Email Services"**
2. Click **"Add New Service"**
3. Choose **"Gmail"**
4. Connect your Gmail account: **selvidesai18@gmail.com**
5. Click **"Create Service"**
6. **Copy the Service ID** (looks like: `service_xxxxx`)

#### **Step 3: Create Email Template**
1. Go to **"Email Templates"**
2. Click **"Create New Template"**
3. Use these settings:

**Template Name:** `portfolio_contact`

**Subject:** `Portfolio Contact: {{from_name}}`

**Content:**
```
From: {{from_name}}
Email: {{from_email}}
Budget/Timeline: {{budget}}

Message:
{{message}}

---
Reply to: {{reply_to}}
```

4. Click **"Save"**
5. **Copy the Template ID** (looks like: `template_xxxxx`)

#### **Step 4: Get Public Key**
1. Go to **"Account"** → **"General"**
2. Find **"Public Key"**
3. **Copy the Public Key** (looks like: `xxxxxxxxxxxxx`)

#### **Step 5: Update Your Code**
Open `main.html` and find these lines (around line 1020):

```javascript
const serviceID = 'YOUR_SERVICE_ID';
const templateID = 'YOUR_TEMPLATE_ID';
const publicKey = 'YOUR_PUBLIC_KEY';
```

Replace with your actual values:
```javascript
const serviceID = 'service_abc123';  // Your Service ID
const templateID = 'template_xyz789'; // Your Template ID
const publicKey = 'abcdefghijklmnop'; // Your Public Key
```

Also update line ~1005:
```javascript
emailjs.init("YOUR_PUBLIC_KEY"); // Replace with your Public Key
```

#### **Step 6: Test It!**
1. Open `main.html` in browser
2. Fill out contact form
3. Click "Send message"
4. Check your Gmail inbox!

---

### **Option 2: Gmail Direct Link (Fallback - Already Working)**

If you don't want to set up EmailJS, the form will automatically open Gmail with pre-filled information.

**How it works:**
- User fills form
- Clicks "Send message"
- Gmail opens with all details pre-filled
- User clicks "Send" in Gmail

**No setup needed!** This already works.

---

## 📝 Current Status

### ✅ **"Let's connect" Button:**
- **Fixed!** Now opens Gmail webmail
- Pre-fills: To: selvidesai18@gmail.com
- Subject: "Portfolio Contact"
- Ready to type message

### ✅ **Contact Form:**
- **Option 1:** EmailJS (automatic) - Requires 5 min setup
- **Option 2:** Gmail link (manual) - Works immediately

---

## 🎯 What Happens Now:

### **When User Clicks "Let's connect":**
```
User clicks button
    ↓
Gmail opens in new tab
    ↓
To: selvidesai18@gmail.com (pre-filled)
    ↓
User types message and sends
    ↓
Email reaches your Gmail inbox ✅
```

### **When User Submits Contact Form:**

**If EmailJS is configured:**
```
User fills form → Clicks "Send message"
    ↓
EmailJS sends email automatically
    ↓
Email reaches selvidesai18@gmail.com ✅
    ↓
User sees "Message sent successfully!"
```

**If EmailJS NOT configured (fallback):**
```
User fills form → Clicks "Send message"
    ↓
Gmail opens with pre-filled details
    ↓
User clicks "Send" in Gmail
    ↓
Email reaches selvidesai18@gmail.com ✅
```

---

## 🔧 Troubleshooting

### **"Let's connect" button not opening Gmail?**
- Make sure you're using Chrome/Edge/Firefox
- Check if pop-ups are blocked
- Try clicking the button again

### **Contact form not sending?**
- **If using EmailJS:** Check that Service ID, Template ID, and Public Key are correct
- **If using fallback:** Make sure Gmail opens (check pop-up blocker)

### **Emails not reaching inbox?**
- Check spam folder
- Verify email: selvidesai18@gmail.com is correct
- If using EmailJS, check EmailJS dashboard for errors

---

## 📧 Email Format

When someone contacts you, you'll receive:

**Subject:** Portfolio Contact: [Name]

**Body:**
```
From: [Name]
Email: [Email]
Budget/Timeline: [Budget]

Message:
[Their message]

---
Reply to: [Email]
```

---

## ✅ Summary

1. ✅ **"Let's connect" button** → Opens Gmail (FIXED)
2. ✅ **Contact form** → Sends to selvidesai18@gmail.com (FIXED)
3. ⚙️ **EmailJS setup** → Optional (for automatic sending)
4. ✅ **Gmail fallback** → Works immediately (no setup)

**Both email methods now work!** 🎉







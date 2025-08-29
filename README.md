# Loqal Email Verification

This repository contains the email verification web interface for the Loqal app.

## 🔗 Live Verification Page

**URL**: https://hsinister.github.io/loqal-verify/verify.html

## 🎯 Purpose

When Loqal users sign up, they receive verification emails with links to this page. The page:

1. **Extracts verification token** from URL parameters
2. **Calls Supabase API** to verify the token
3. **Shows success/error message** to the user
4. **Updates user verification status** in the database

## ⚙️ Setup

### 1. Enable GitHub Pages
- Go to **Settings** → **Pages**
- **Source**: Deploy from a branch
- **Branch**: `main`
- **Folder**: `/ (root)`
- **Save**

### 2. Configure Supabase Key ✅
~~Edit `verify.html` and replace both instances of:~~
```javascript
✅ Already configured with your Supabase anon key
```

~~With your Supabase anon key from:~~
~~- [Supabase Dashboard](https://supabase.com/dashboard) → Your Project → Settings → API~~

### 3. Test
Send a verification email from the Loqal app and click the link!

## 🔐 Security

- Uses public Supabase anon key (safe to expose)
- Tokens are single-use and expire in 24 hours
- No sensitive app code is exposed in this repository

## 📱 Loqal App

This verification page is part of the Loqal location discovery app. The main app repository is private for security.

---

**🎯 Loqal** - Discover amazing places around you!

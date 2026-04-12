# 🍽️ AI Meal Planner - Setup Guide

## ✨ What This Is

An intelligent recipe extraction and meal planning system that:
- ✅ Extracts recipes from ANY URL (Instagram, blogs, YouTube)
- ✅ Uses Claude AI to calculate macros automatically
- ✅ Intelligently tags recipes (breakfast/lunch/dinner/pre-workout/post-workout)
- ✅ Stores recipes in your browser (private & offline)
- ✅ Flags uncertain extractions for review
- ✅ Supports multiple URLs at once
- ✅ YouTube playlist support (coming soon)

## 🚀 Quick Start (For You)

### Step 1: Get Claude API Key

1. Go to https://console.anthropic.com
2. Sign up / Log in
3. Go to "API Keys"
4. Create a new key
5. Copy it (starts with `sk-ant-`)

**Cost:** ~$0.001 per recipe (100 recipes = $0.10, 1000 recipes = $1.00)

### Step 2: Deploy to GitHub Pages

1. **Create a new GitHub repository:**
   - Go to https://github.com/new
   - Repository name: `meal-planner`
   - Make it **Public** (so friends can fork it)
   - Click "Create repository"

2. **Upload the file:**
   - Click "uploading an existing file"
   - Drag and drop `meal-planner.html`
   - Commit the file

3. **Enable GitHub Pages:**
   - Go to Settings → Pages
   - Source: Deploy from branch
   - Branch: `main` → folder: `/` (root)
   - Click Save
   
4. **Wait 1-2 minutes**, then your site will be live at:
   ```
   https://YOUR-USERNAME.github.io/meal-planner/meal-planner.html
   ```

### Step 3: Configure API Key

1. Open your deployed site
2. Click "⚙️ Settings"
3. Paste your Claude API key
4. Click "Save Settings"

### Step 4: Extract Your First Recipe!

1. Click "📥 Extract Recipes"
2. Paste recipe URLs (comma-separated):
   ```
   https://example.com/recipe1, https://example.com/recipe2
   ```
3. Click "🤖 Extract Recipes with AI"
4. Wait for extraction (progress bar will show)
5. View extracted recipes!

---

## 👥 For Friends - How to Get Your Own Copy

### Method 1: Fork the Repository (Recommended)

1. **Fork the repo:**
   - Go to https://github.com/YOUR-USERNAME/meal-planner
   - Click "Fork" (top right)
   - Click "Create fork"

2. **Enable GitHub Pages on YOUR fork:**
   - Go to Settings → Pages
   - Source: Deploy from branch
   - Branch: `main` → folder: `/` (root)
   - Click Save

3. **Your own copy is now live at:**
   ```
   https://YOUR-FRIEND-USERNAME.github.io/meal-planner/meal-planner.html
   ```

4. **Add your own API key:**
   - Open your site
   - Go to Settings
   - Add your Claude API key
   - Your recipes are completely separate!

### Method 2: Download and Use Locally

1. Download `meal-planner.html`
2. Open it in any browser
3. Add your API key in Settings
4. Start extracting recipes!

**No server needed - works 100% offline!**

---

## 📖 How to Use

### Extracting Recipes

**Single URL:**
```
https://foodblog.com/amazing-curry
```

**Multiple URLs (comma-separated):**
```
https://blog1.com/recipe1, https://blog2.com/recipe2, https://instagram.com/p/abc123
```

**YouTube Videos:**
```
https://youtube.com/watch?v=abc123, https://youtube.com/watch?v=xyz789
```

**YouTube Playlists:**
```
https://youtube.com/playlist?list=PLxxx
```
_(Will show video list, you check which ones to extract)_

### Supported Sources

- ✅ Food blogs (any website)
- ✅ Instagram posts/reels
- ✅ YouTube videos
- ✅ YouTube playlists (manual selection)
- ✅ Recipe websites
- ✅ Any URL with recipe content

### What Gets Extracted

For each recipe:
- 📝 Recipe name
- 🔗 Source URL
- 🥘 Ingredients list
- 📊 Macros (calories, protein, carbs, fat, fiber)
- 🍽️ Serving size
- 🏷️ Auto-tags:
  - Meal type (breakfast/lunch/dinner)
  - Workout timing (pre-workout/post-workout)
  - Intensity (light/medium/heavy)
  - Complexity (simple/moderate/elaborate)

### Uncertainty Flags

If AI is uncertain about macros, you'll see:
```
⚠️ Macros may need review: [reason]
```

You can edit these manually in your library.

---

## 🎯 Features

### Current Features (Live Now!)

✅ **AI Recipe Extraction**
- Paste any URL
- Claude AI reads and extracts
- Calculates macros from ingredients
- Intelligent auto-tagging

✅ **Recipe Library**
- View all saved recipes
- Search and filter
- Edit tags later
- Delete recipes

✅ **Progress Tracking**
- Real-time extraction progress
- Multiple recipe support
- Success/error notifications

✅ **Data Management**
- Export recipes (JSON)
- Import recipes (JSON)
- Share with friends
- Clear all data

✅ **Privacy**
- All data in browser only
- No cloud storage
- Works offline
- Completely private

### Coming Soon

🔜 **YouTube Playlist Support**
- Automatic video list extraction
- Select which videos to process
- Batch extraction

🔜 **Manual Recipe Editing**
- Edit macros if AI got them wrong
- Adjust tags and serving sizes
- Update recipe details

🔜 **Meal Planner**
- Plan weekly meals
- Activity-based slot generation
- Smart timing warnings
- Macro tracking

🔜 **Cloud Sync (Optional)**
- Access from any device
- Share libraries with friends
- Backup in cloud

---

## 💡 Pro Tips

### Getting Better Extractions

1. **Use recipe URLs with clear ingredient lists**
   - Food blogs work best
   - Instagram captions with ingredients
   - YouTube descriptions with ingredients

2. **For Instagram:**
   - Make sure caption has ingredients
   - Or paste the text separately

3. **For YouTube:**
   - Check description for ingredients
   - Or use timestamped descriptions

### Managing Your Library

1. **Export regularly** - Download JSON backup
2. **Review uncertain macros** - Check flagged recipes
3. **Edit tags** - Adjust AI suggestions
4. **Search efficiently** - Use search box

### Sharing with Friends

1. **Share your GitHub repo** - They can fork
2. **Export recipes** - Share JSON file
3. **Each person gets own data** - No overlap

---

## 🔧 Troubleshooting

### "Please set your Claude API key"

**Solution:**
1. Go to Settings tab
2. Paste your API key (starts with `sk-ant-`)
3. Click Save Settings

### "API error: 401"

**Solution:** Invalid API key
- Check you copied the full key
- Make sure key is active in console.anthropic.com

### "API error: 429"

**Solution:** Rate limit exceeded
- Wait a few minutes
- Extract fewer recipes at once

### "Failed to extract recipe"

**Possible reasons:**
- URL doesn't contain a recipe
- Page requires login
- Format not recognized

**Solution:**
- Try a different URL
- Copy-paste recipe text manually
- Check if page loads in browser

### Recipes not showing in library

**Solution:**
- Check console for errors (F12)
- Clear browser cache
- Refresh the page

---

## 📊 Cost Calculator

Based on Claude API pricing:

| Recipes | Cost |
|---------|------|
| 10 | $0.01 |
| 50 | $0.05 |
| 100 | $0.10 |
| 500 | $0.50 |
| 1,000 | $1.00 |
| 5,000 | $5.00 |

**Very affordable!** Most users extract 50-200 recipes total.

---

## 🔐 Privacy & Security

### What's Stored Where

**In Your Browser (localStorage):**
- Your recipes
- Your API key (encrypted in browser)
- Your settings

**Sent to Claude API:**
- Recipe URLs (to extract content)
- Recipe text (to analyze)

**Never Stored in Cloud:**
- Your recipes (unless you enable cloud sync later)
- Your personal data

### Is It Safe?

✅ **Your API key** - Stored only in your browser
✅ **Your recipes** - Stay on your device
✅ **No tracking** - No analytics, no cookies
✅ **Open source** - Code is visible on GitHub

---

## 🆘 Support

### Getting Help

1. **Check this README** - Most answers are here
2. **Check console** - F12 → Console tab for errors
3. **GitHub Issues** - Report bugs or ask questions

### Updating to Latest Version

When updates are available:

**If you forked:**
1. Go to your fork
2. Click "Sync fork"
3. Click "Update branch"
4. Wait for GitHub Pages to redeploy

**If downloaded locally:**
1. Download new version
2. Replace old file
3. Refresh browser

---

## 🎉 Next Steps

After setting up:

1. ✅ Extract 5-10 favorite recipes
2. ✅ Review and edit tags
3. ✅ Export a backup
4. ✅ Share with friends!

---

## 📝 Changelog

### Version 1.0 (Current)
- ✅ AI recipe extraction
- ✅ Multi-URL support
- ✅ Auto-tagging
- ✅ Recipe library
- ✅ Search & filter
- ✅ Export/Import
- ✅ Progress tracking
- ✅ Uncertainty flagging

---

**Built with ❤️ for sustainable meal planning**

Questions? Check the GitHub repo or create an issue!

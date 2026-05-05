# Luminary 🕯️
**One Light**

Daily spiritual wisdom from Christian teachings. One meaningful offering, delivered once a day.

---

## 📁 Files in This Project

- `index.html` - The main app
- `quotes.json` - Database of 240 Christian quotes
- `manifest.json` - PWA configuration
- `luminary_privacy.html` - Privacy policy
- `icon.png` - App icon (512x512px)
- `README.md` - This file

---

## 🚀 Deploying to GitHub Pages

### Step 1: Create GitHub Repository
1. Go to https://github.com
2. Click **"New repository"** (green button)
3. Repository name: `luminary` (or whatever you want)
4. Make it **Public**
5. **DO NOT** check "Add a README file"
6. Click **"Create repository"**

### Step 2: Upload Files
**Option A: Upload via Web Interface** (Easiest!)
1. On your new repository page, click **"uploading an existing file"**
2. Drag ALL these files into the upload box:
   - index.html
   - quotes.json
   - manifest.json
   - luminary_privacy.html
   - icon.png
3. Scroll down, write commit message: "Initial Luminary app"
4. Click **"Commit changes"**

**Option B: Via Command Line** (If you know Git)
```bash
git init
git add .
git commit -m "Initial Luminary app"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/luminary.git
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. In your repository, click **"Settings"** tab
2. Scroll down to **"Pages"** in left sidebar
3. Under "Source", select **"Deploy from a branch"**
4. Under "Branch", select **"main"** and **"/ (root)"**
5. Click **"Save"**
6. Wait 2-3 minutes
7. Your site will be live at: `https://YOUR-USERNAME.github.io/luminary/`

---

## 📝 How to Update Quotes

### Adding More Christian Quotes

1. Open `quotes.json` in any text editor
2. Add new quotes at the end of the array:

```json
{
  "id": 241,
  "quote": "Your new quote text here",
  "speaker": "Speaker Name",
  "reference": "Book Chapter:Verse",
  "subject": "Hope",
  "religion": "Christian",
  "religion_order": 5,
  "path": "Evangelical",
  "subject_order": 25
}
```

3. Save the file
4. Commit and push to GitHub:
   - **Via Web**: Click on `quotes.json` → Edit → Make changes → Commit
   - **Via Command Line**: `git add quotes.json`, `git commit -m "Added more quotes"`, `git push`

5. Changes go live automatically in 1-2 minutes!

### Important Notes:
- Each quote needs a unique `id` (just increment from the last one)
- `religion` should be "Christian" for now
- `religion_order` should be 5 for all Christian quotes
- `path` can be: "Evangelical", "Mystic", "Orthodox", or "Quaker"
- `subject_order` is the sequence number within that Subject (Hope 1, Hope 2, etc.)

---

## 🔄 Adding Jewish Quotes (Future)

When you're ready to add Jewish quotes:

1. Add them to `quotes.json` with:
   - `religion`: "Jewish"
   - `religion_order`: 10
   - `path`: "" (leave empty)
   - `subject_order`: Start at 1 for each subject

2. The app will automatically start transitioning when users hit 85% of Christian quotes!

---

## 📱 Google Play Store

After deploying to GitHub Pages, you can submit the web app to Google Play as a TWA (Trusted Web Activity).

See `GOOGLE_PLAY_GUIDE.md` for step-by-step instructions.

---

## 🎨 Customization

### Change Colors
Edit the `:root` section in `index.html`:
```css
:root {
  --gold: #c8a45a;  /* Main accent color */
  --bg: #141210;    /* Background */
}
```

### Change Icon
Replace `icon.png` with your own 512x512px PNG image.

---

## 📊 Current Stats

- **Total quotes**: 240
- **Subjects**: 64
- **Duration**: ~8 months of daily content

---

## 🆘 Troubleshooting

**Site not loading?**
- Check that GitHub Pages is enabled in Settings → Pages
- Make sure all files are in the root directory (not in a subfolder)
- Wait 2-3 minutes after enabling Pages

**Quotes not showing?**
- Check browser console (F12) for errors
- Make sure `quotes.json` is valid JSON (use jsonlint.com to validate)

**Need to reset a user's progress?**
- Open browser console (F12)
- Type: `localStorage.clear()`
- Refresh the page

---

## 📧 Support

Questions? Issues? Contact via mPoPtop.com

---

**Built with ❤️ for daily spiritual wisdom**

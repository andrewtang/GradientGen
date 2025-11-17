# GradientGen - Free Hosting Guide

## 🚀 Free Hosting Options

Your application is a static web app that can be hosted for free on several platforms.

### Option 1: GitHub Pages (Easiest!)

**Steps:**

1. **Create a GitHub account** (if you don't have one): https://github.com

2. **Create a new repository**:
   - Click on "New repository"
   - Name it (e.g., `gradientgen`)
   - Choose "Public"
   - Click on "Create repository"

3. **Upload your files**:
   - Download GitHub Desktop: https://desktop.github.com
   - Or use the following commands in your terminal:

```bash
cd "C:\Users\noega\Desktop\FreeTool1"
git init
git add .
git commit -m "First version"
git branch -M main
git remote add origin https://github.com/YOUR-NAME/gradientgen.git
git push -u origin main
```

4. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click on "Settings"
   - In the left menu, click on "Pages"
   - Under "Source", select "main" (or "master")
   - Click on "Save"
   - Your site will be available at: `https://YOUR-NAME.github.io/gradientgen`

### Option 2: Netlify (Very simple with drag & drop!)

**Steps:**

1. **Go to Netlify**: https://www.netlify.com
2. **Create a free account** (with GitHub, Google, or email)
3. **Drag and drop your folder** `FreeTool1` onto the Netlify page
4. **That's it!** You get a URL immediately

**Advantages:**
- Custom URL (e.g., `your-name.netlify.app`)
- Automatic deployment if you use Git
- Free HTTPS
- Very fast

### Option 3: Vercel (Excellent performance)

**Steps:**

1. **Go to Vercel**: https://vercel.com
2. **Create a free account**
3. **Import your project** (via GitHub or drag & drop)
4. **Deploy!**

### Option 4: Cloudflare Pages

**Steps:**

1. **Go to Cloudflare Pages**: https://pages.cloudflare.com
2. **Create a free account**
3. **Connect your GitHub repository** or upload manually
4. **Deploy!**

## 📁 File Structure

Your application contains:
- `index.html` - Main page
- `sketch.js` - JavaScript code (now contains the embedded shader)
- `styles.css` - CSS styles
- `Image.frag` - WebGL shader (optional, now embedded in sketch.js)
- `BergenMono-Regular.otf` - Font file

**Important note:** The `Image.frag` shader is now embedded directly in `sketch.js` to avoid CORS issues when opening locally (file://). The application now works even if you simply open the HTML file in your browser without a web server!

All these files must be in the same folder at the root.

## ⚡ Updating

To update your site:

**GitHub Pages:**
- Modify your files locally
- Commit and push to GitHub
- The site updates automatically in a few minutes

**Netlify/Vercel:**
- If connected to GitHub: automatic push
- Otherwise: drag and drop your updated folder again

## 🌐 Share Your URL

Once deployed, you can share the URL with anyone!

## 💡 Tip

For a custom domain name (optional, free on some services):
- Netlify and Vercel allow you to add a custom domain for free
- You can also use a free subdomain on Freenom

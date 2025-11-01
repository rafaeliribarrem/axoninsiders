# Axon Insiders - Webflow Scripts

This repository contains custom JavaScript files for Webflow integration via jsDelivr CDN.

## 🚀 Quick Start

### 1. Set up GitHub Repository

1. Create a new repository on GitHub (if you haven't already)
2. Push this code to your repository
3. Note your GitHub username and repository name

### 2. Get Your jsDelivr CDN Link

Once your code is on GitHub, you can use jsDelivr to serve it:

```
https://cdn.jsdelivr.net/gh/USERNAME/REPO@BRANCH/FILENAME.js
```

**Example:**

```
https://cdn.jsdelivr.net/gh/yourusername/axon-insiders@main/scripts.js
```

### 3. Add to Webflow

1. Open your Webflow project
2. Go to **Project Settings** > **Custom Code**
3. Paste your jsDelivr link in the **Footer Code** section:
   ```html
   <script src="https://cdn.jsdelivr.net/gh/yourusername/axon-insiders@main/scripts.js"></script>
   ```
4. Click **Save**

## 📝 Making Changes

### Easy Git Workflow

1. **Make your changes** to `scripts.js`
2. **Stage changes:**
   ```bash
   git add scripts.js
   ```
3. **Commit:**
   ```bash
   git commit -m "Description of your changes"
   ```
4. **Push to GitHub:**
   ```bash
   git push origin main
   ```

The changes will be live on jsDelivr immediately (or within a few minutes).

### Pro Tips

- **Use version tags** for stable releases:
  ```
  https://cdn.jsdelivr.net/gh/USERNAME/REPO@v1.0.0/scripts.js
  ```
- **Use branches** for testing:
  ```
  https://cdn.jsdelivr.net/gh/USERNAME/REPO@develop/scripts.js
  ```
- **Minify your code** before committing for better performance
- **Test changes** in a staging branch before pushing to main

## 📁 File Structure

```
.
├── scripts.js          # Main JavaScript file
├── README.md          # This file
└── .gitignore        # Git ignore file
```

## 🔧 Initial Git Setup

If this is a new repository, run these commands:

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/USERNAME/REPO.git
git branch -M main
git push -u origin main
```

Replace `USERNAME` and `REPO` with your actual GitHub username and repository name.

## ⚡ Performance Optimizations

The code has been optimized for better performance:

### Key Improvements:

- **Debounced resize handlers** - Prevents excessive function calls on window resize
- **Throttled mouse events** - Optimizes cursor movement to ~60fps
- **Event delegation** - Reduces memory footprint by using event bubbling
- **DocumentFragment** - Batch DOM operations for grid generation
- **Cached DOM queries** - Reduces repeated selector calls
- **Passive event listeners** - Improves scroll performance
- **Single MutationObserver** - More efficient DOM mutation watching
- **Lazy Three.js loading** - Only loads when needed
- **One-time event listeners** - Uses `{ once: true }` where appropriate
- **Transform instead of left/top** - Better GPU acceleration for cursor

### Features Included:

✅ Custom cursor with hover states
✅ Hamburger menu toggle
✅ Page transition grid system
✅ Three.js CRT effect (with mobile optimizations)
✅ Pixelate reveal animation
✅ Typewriter effect
✅ SVG flash animation
✅ Pixel burst effect

All functionality preserved while improving performance!

## 📚 Resources

- [jsDelivr Documentation](https://www.jsdelivr.com/documentation)
- [GitHub Pages Alternative](https://pages.github.com/)
- [Webflow Custom Code](https://university.webflow.com/lesson/add-custom-code-to-your-site)

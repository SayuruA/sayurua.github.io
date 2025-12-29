# How to Add Your Custom Favicon

## What is a Favicon?
A favicon is the small icon that appears in browser tabs, bookmarks, and browser history next to your website's title.

## Steps to Add Your Custom Favicon:

### 1. Prepare Your Icon Image
- Create or find an image you want to use as your favicon
- Recommended formats: `.ico`, `.png`, or `.svg`
- Recommended sizes:
  - **favicon.ico**: 16x16, 32x32, or 48x48 pixels (can contain multiple sizes)
  - **favicon.png**: 32x32 or 192x192 pixels
  - **favicon.svg**: Vector format (scalable)

### 2. Place Your Favicon File
Save your favicon file in this directory (`/static/`) with one of these names:
- `favicon.ico` (most compatible)
- `favicon.png` (modern browsers)
- `favicon.svg` (best quality, modern browsers)

**Important:** The file MUST be named exactly `favicon.ico` (or `.png`/`.svg`) and placed directly in the `/static/` folder.

### 3. Update Configuration (if using a different name)
If you want to use a different filename or format, edit `hugo.toml` and change this line:
```toml
favicon = "/favicon.ico"
```
to:
```toml
favicon = "/your-custom-name.png"  # or .svg
```

### 4. Rebuild Your Site
After adding the favicon file:
- If Hugo is running in dev mode (`hugo server`), it should auto-reload
- Otherwise, run `hugo` to rebuild the site
- Clear your browser cache or do a hard refresh (Ctrl+F5) to see the new icon

## Online Tools to Create Favicons:
- **favicon.io** - https://favicon.io/ (convert images, text, or emojis to favicons)
- **RealFaviconGenerator** - https://realfavicongenerator.net/ (comprehensive favicon generator)
- **Canva** - Create a simple icon design and export as PNG

## Current Configuration:
✅ Your site is configured to use: `/favicon.ico`
📁 Place your file here: `c:\Users\SAYURU SHENAL\OneDrive - University of Moratuwa\Documents\UoM\Important\myweb\static\favicon.ico`

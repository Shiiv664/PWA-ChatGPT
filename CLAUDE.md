# ChatGPT PWA Project

## Project Overview
Progressive Web App that redirects to ChatGPT with custom icon and standalone window behavior.

## Project Structure
```
/home/shiiv/dev/chatgpt-pwa/
├── index.html          # Main HTML file with ChatGPT redirect
├── manifest.json       # Web app manifest with custom icon
├── sw.js              # Minimal service worker for PWA requirements
└── icons/
    ├── icon-192.png   # 192x192 app icon
    └── icon-512.png   # 512x512 app icon
```

## Tools Used (ARM64 Compatible)
- **ImageMagick**: `sudo apt install imagemagick` - Image processing and conversion
- **librsvg2-bin**: `sudo apt install librsvg2-bin` - SVG to PNG conversion with rsvg-convert

## Commands for This Project
- **SVG to PNG conversion**: `rsvg-convert -w 192 -h 192 input.svg -o output.png`
- **Local HTTP server**: `python3 -m http.server 8080` - Serves current directory on localhost:8080
- **Test PWA**: Navigate to `http://localhost:8080` in Chrome

## Installation Instructions
1. Run `python3 -m http.server 8080` from project directory
2. Open `http://localhost:8080` in Chrome
3. Click "Install app" icon in address bar
4. Enjoy your custom ChatGPT PWA!

## Features
- Custom ChatGPT icon (better than browser default)
- Standalone app window (not browser tabs)
- Seamless redirect to ChatGPT
- PWA-compliant with service worker
- ARM Chromebook compatible
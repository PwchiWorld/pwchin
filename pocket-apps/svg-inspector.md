# SVG Inspector Pro

A lightweight, client-side web application for visually inspecting, editing, and optimizing SVG files. Paste any SVG code, toggle elements visibility, change colors in real-time, and export optimized versions.

![SVG Inspector Pro Interface](https://via.placeholder.com/800x400/2c3e50/ffffff?text=SVG+Inspector+Pro+Interface)

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://pwchiworld.github.io/svg-inspector-pro)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![SVG](https://img.shields.io/badge/SVG-optimization-orange)

## ?? Overview

**SVG Inspector Pro** solves a common problem when working with complex or non-standard SVG files: understanding structure and making quick visual adjustments. Instead of manually editing code, you can:

- **Visualize** all SVG elements with ID attributes
- **Toggle** visibility of specific elements
- **Change** fill colors with a color picker
- **Export** cleaned SVG with only visible elements
- **Minify** output for production use
- **Download** as PNG raster image

## ? Key Features

| Feature | Description |
|---------|-------------|
| **Element Inspector** | Automatically detects all elements with IDs and creates toggle controls |
| **Live Color Picker** | Change fill colors of individual elements instantly |
| **Visibility Toggle** | Hide unwanted elements (they're removed from export) |
| **Smart Preview** | Hover controls highlight corresponding elements in preview |
| **Dual Export** | Standard SVG or minified version (removes comments, whitespace) |
| **PNG Export** | Rasterize SVG to PNG at 2x resolution |

## ?? How It Works

1. **Paste** your SVG code into the textarea
2. **Click** "Load SVG" to parse and inspect
3. **Toggle** switches to hide/show elements
4. **Pick** colors to modify appearance
5. **Export** as SVG (regular or minified) or PNG

The tool works entirely in your browser - no server uploads, no data leaves your machine.

## ?? Use Cases

- **Icon Libraries**: Clean up icon sets by removing unused layers
- **Illustration Editing**: Quickly change colors without opening design software
- **SVG Optimization**: Remove hidden elements and minify for web use
- **Debugging**: Understand structure of complex, poorly formatted SVGs
- **Batch Preparation**: Visually inspect and prepare SVGs for development

## ??? Technical Details

- Pure HTML/CSS/JavaScript - no dependencies
- Works offline - save the HTML file locally
- Client-side processing - privacy focused
- Handles non-standard SVG structures gracefully
- Responsive design works on mobile devices

## ?? Interface Guide

- **Left Panel**: SVG input area, filename input, and list of all elements with IDs
- **Right Panel**: Live preview with sticky controls, export buttons
- **Element Controls**: Each ID gets a toggle switch and color picker
- **Hover Effect**: Mouse over any control to highlight corresponding element

## ?? Usage Example

```
html
<!-- Paste complex SVG like this -->
<svg viewBox="0 0 100 100">
  <g id="background">
    <rect id="bg-rect" width="100" height="100" fill="blue"/>
  </g>
  <circle id="main-dot" cx="50" cy="50" r="20" fill="red"/>
  <path id="decoration" d="M20 80 L80 20" stroke="green"/>
</svg>
```
Then toggle off decoration, change bg-rect to purple, export minified - all visually!

## ?? Live Demo
Try it online: ![SVG Inspector Pro Demo](https://img.shields.io/badge/JavaScript-ES6-yellow)
Download this file: ![Download SVG Inspector Pro Demo](https://img.shields.io/badge/JavaScript-ES6-yellow)



## ?? Local Installation
Download the HTML file

1. Open in any modern browser
2. Start pasting SVGs!
3. No build process, no npm install, no configuration needed.

## ?? Notes
Elements without IDs won't appear in the controls list

* Changes are non-destructive - original code remains in textarea
* Color picker defaults to gray if fill detection fails
* PNG export uses canvas at 2x resolution for better quality

## ?? Customization
Feel free to modify the code:

* Adjust gradient backgrounds in the CSS
* Add more export formats (JPG, WebP)
* Implement search/filter for elements
* Add attribute editing beyond fill color

## ?? License
MIT - Use freely in personal and commercial projects
# 🔐 DarkWeb Checker

A powerful web-based security audit tool to identify compromised passwords in your Bitwarden vault by matching them against dark web leak patterns.

## Features

- 📂 **Pattern Matching** - Add password patterns (e.g., `fuc•••••`) to identify compromised credentials
- 🎯 **Live Analysis** - Real-time detection as you paste patterns
- 📊 **Compact Cards** - View all matched entries in an organized grid layout
- 📁 **Collapsible Folders** - Group results by pattern with expand/collapse functionality
- 🙈 **Ignore Tracking** - Mark passwords as resolved with a simple checkbox
- 💛 **Visual Tracking** - Highlight entries with yellow glow for easy identification
- 💾 **JSON Persistence** - Save your progress directly in the JSON file (`_ignored` field)
- 📅 **Timestamps** - See when each entry was created (dd/mm/yyyy format)
- 🔑 **Password Display** - View the actual compromised password for each site
- 🔗 **Clickable Links** - Direct access to each website

## Quick Start

1. **Export your Bitwarden vault** as JSON
2. **Open the HTML file** in your browser
3. **Import the JSON** using the import button
4. **Paste patterns** in the left panel (one per line, format: `w••••` or `gja••••••••`)
5. **View results** organized by pattern
6. **Click vignettes** to highlight them while working through them
7. **Check Ignore** to mark passwords as resolved
8. **Save Progress** to download your updated JSON with ignored entries

## Pattern Format

Patterns represent a password's prefix and total length using bullet characters:

- `fuc•••••` = starts with "fuc", 6 characters total
- `w••••` = starts with "w", 5 characters total
- `gja••••••••` = starts with "gja", 10 characters total

**Case-sensitive matching** - patterns must match exactly.

## UI Guide

- **Left Panel**: Pattern input and ignored items counter
- **Stats Cards**: At-risk count, safe count, total, and risk percentage
- **Folders**: Click to expand/collapse patterns, use ━ icon to minimize
- **Cards**: 
  - Click anywhere to highlight with yellow glow (one at a time)
  - Click link to visit the website
  - Click 🙈 to mark as ignored
  - All data in the card: site name, folder, date, password

## Data Storage

- **All data stays local** - nothing is sent anywhere
- **Ignored entries** are stored in the JSON's `_ignored` field
- **Tracking highlights** (glow) exist only during your session
- **Save Progress** downloads the updated JSON file

## Browser Compatibility

Works on all modern browsers with ES6 support (Chrome, Firefox, Safari, Edge)

## Features Breakdown

| Feature | Status |
|---------|--------|
| Pattern matching | ✅ |
| Live analysis | ✅ |
| Password visibility | ✅ |
| Ignore tracking | ✅ |
| Visual highlighting | ✅ |
| JSON persistence | ✅ |
| Responsive design | ✅ |
| Glassmorphism UI | ✅ |

## Tips

- **Organize by pattern**: Expand one pattern at a time to stay focused
- **Track your progress**: Use the yellow glow to remember which entries you're analyzing
- **Check before ignoring**: Always verify a password is safe before marking it ignored
- **Save regularly**: Use Save Progress to backup your work
- **Scroll freely**: All vignettes are scrollable - no internal scroll limits

## License

Open source - feel free to use and modify

## Disclaimer

This tool is for security auditing your own Bitwarden vault only. Always verify entries before marking them as resolved. Keep your password vault secure.
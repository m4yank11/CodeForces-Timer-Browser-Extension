﻿# Codeforces Timer Extension

A Chrome extension that adds a customizable timer to Codeforces problem pages to help users track their problem-solving time.

## Features

- Built-in timer presets (5, 10, 15, 20, 25, and 30 minutes)
- Timer appears directly on Codeforces problem pages
- Automatic detection of problem completion
- Visual timer state indicators (Running, Finished, Timed Out)
- Local storage to persist timer state across page reloads

## Installation

1. Clone this repository or download the zip file
2. Open Chrome and navigate to `chrome://extensions/`
3. Enable "Developer mode" in the top right corner
4. Click "Load unpacked" and select the `cf-timer` folder

## Usage

1. Click the extension icon in your browser toolbar to select a timer duration
2. Choose from preset times or set a custom duration
3. Navigate to any Codeforces problem page to see the timer in action
4. The timer will automatically:
   - Start counting down
   - Show "Finished" when the problem is solved
   - Display "Timed Out" when time expires

## Controls

- **Pause**: Temporarily stop the timer
- **Reset**: Reset the timer to its initial value
- **Custom Timer**: Set specific hours and minutes

## Permissions

The extension requires:
- `storage`: To save timer preferences and state
- Access to Codeforces problem pages:
  - `https://codeforces.com/problemset/problem/*`
  - `https://codeforces.com/contest/*/*`

## Files Structure

```
cf-timer/
├── manifest.json      # Extension configuration
├── css/
│   ├── popup.css     # Popup styling
│   └── styles.css    # Timer styling
├── html/
│   └── popup.html    # Timer selection popup
├── js/
│   ├── background.js # Background timer logic
│   ├── content.js    # Page integration code
│   └── popup.js      # Popup interaction logic
└── images/
    ├── cftimer.png   # Extension icon
    └── codeforces.png
```

# POE2 Act Guide

An interactive web-based guide for Path of Exile 2 acts with progress tracking and persistent state management.

## Features

- **Collapsible Act Sections** - Expand/collapse acts to focus on specific content
- **Progress Tracking** - Check off completed steps and objectives with visual feedback
- **Dark/Light Mode** - Toggle between dark and light themes
- **Persistent State** - All progress, theme preference, and section states are saved in your browser
- **Clean, Minimal Design** - Simple black, white, and gray styling focused on readability

## How to Use

1. Open `index.html` in your web browser
2. Click on act headers to expand/collapse sections
3. Check boxes next to steps and objectives as you progress
4. Toggle between dark and light mode using the buttons in the header
5. Your progress is automatically saved - reload the page anytime and your state is restored

## Technology Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom styling with CSS variables for theming
- **Vanilla JavaScript** - No dependencies
- **XML** - Data structure for guide content
- **localStorage** - Browser-based persistence

## Files

- `index.html` - Main web interface
- `styles.css` - Styling and theming
- `poe2_act_guide.xml` - Guide content structure

## Getting Started

To run locally:

```bash
npx http-server -p 8000
```

Then open `http://localhost:8000` in your browser.

## Data Structure

Guide content is stored in `poe2_act_guide.xml` with the following structure:

```xml
<guide>
  <act number="1">
    <step number="1">
      <name>Location Name</name>
      <objectives>
        <objective>Objective description</objective>
      </objectives>
    </step>
  </act>
  <interludes>
    <!-- Interlude content -->
  </interludes>
</guide>
```

## Browser Compatibility

Works in all modern browsers that support:
- ES6 JavaScript
- CSS Custom Properties (variables)
- localStorage API

## License

Free to use and modify for personal use.

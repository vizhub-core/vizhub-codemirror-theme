# vizhub-codemirror-theme

A custom CodeMirror 6 theme designed for VizHub, providing a modern and visually appealing syntax highlighting experience.

## Installation

```bash
npm install @vizhub/codemirror-theme
```

## Usage

```javascript
import { vizhubTheme } from "@vizhub/codemirror-theme";
import { EditorView } from "codemirror";

// Use in CodeMirror setup
new EditorView({
  extensions: [vizhubTheme],
  // ... other configuration
});
```

## Features

- Modern, carefully chosen color palette
- Optimized for readability and visual hierarchy
- Support for matching/non-matching bracket highlighting
- Semi-bold weight for keywords and important syntax elements
- Customized colors for:
  - Keywords and operators
  - Strings and numbers
  - Functions and variables
  - Comments and metadata
  - And more...

## Customization

You can customize the theme by using the underlying `vizhubThemeInit` function:

```javascript
import { vizhubThemeInit } from "@vizhub/codemirror-theme";

const customizedTheme = vizhubThemeInit({
  theme: "dark", // or 'light'
  settings: {
    // Override default settings
  },
  styles: [
    // Add custom styles
  ],
});
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT © [Curran Kelleher](https://github.com/curran)

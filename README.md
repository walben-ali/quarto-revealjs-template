# Quarto Reveal.js Presentation Template

A comprehensive template for creating professional presentations using Quarto and Reveal.js.

## Project Structure

```
.
├── index.qmd              # Main presentation file with slide content
├── _quarto.yml            # Quarto project configuration
├── custom.css             # Custom styling and theme
├── references.bib         # Bibliography for citations
├── logo.png               # (Optional) Logo image for slides
└── README.md              # This file
```

## Files Overview

### index.qmd
The main presentation file containing:
- YAML front matter with metadata
- Multiple slide examples
- Various slide layouts (columns, incremental, etc.)
- Code examples with syntax highlighting
- Callout boxes and emphasis
- Speaker notes
- Mathematical equations

### _quarto.yml
Quarto project configuration including:
- Theme settings
- Reveal.js options (transitions, animations, etc.)
- Chalkboard plugin configuration
- Code highlighting preferences
- PDF export settings
- Slide dimensions and margins

### custom.css
Comprehensive CSS styling featuring:
- Custom color variables
- Typography and heading styles
- Code block and table styling
- Callout box designs
- Responsive design
- Dark mode support
- Print-friendly styles

## Getting Started

### Prerequisites
- [Quarto](https://quarto.org/docs/get-started/) installed
- A text editor or IDE (VS Code, RStudio, etc.)

### Installation

1. Clone or download this repository
2. Navigate to the project directory
3. Install Quarto if not already installed

### Building and Previewing

```bash
# Preview the presentation
quarto preview index.qmd

# Render to HTML
quarto render index.qmd

# Render to PDF
quarto render index.qmd --to pdf
```

## Customization

### Changing Colors
Edit the CSS variables in `custom.css`:

```css
:root {
  --primary-color: #2c3e50;
  --secondary-color: #3498db;
  --accent-color: #e74c3c;
  /* ... other colors ... */
}
```

### Modifying Themes
Update the `format.revealjs.theme` in `_quarto.yml`:

```yaml
format:
  revealjs:
    theme: [default, custom.css]  # Change default to: dark, simple, black, league, etc.
```

### Adding Logos and Footers
Set in the YAML front matter or `_quarto.yml`:

```yaml
logo: "path/to/logo.png"
footer: "Your Organization © 2024"
```

### Configuring Transitions
In `_quarto.yml`:

```yaml
transition: slide          # Options: slide, fade, convex, concave, zoom
background-transition: fade
```

## Features

- ✅ Responsive design for all screen sizes
- ✅ Multiple slide layouts and templates
- ✅ Syntax-highlighted code blocks
- ✅ Mathematical equations support
- ✅ Incremental animations and fragments
- ✅ Speaker notes for presenter view
- ✅ Chalkboard for interactive annotations
- ✅ Print-friendly styling
- ✅ Dark mode support
- ✅ Customizable colors and fonts

## Slide Types Included

1. **Title Slide** - Main presentation introduction
2. **Content Slides** - Standard bullet point slides
3. **Two-Column Layouts** - Side-by-side content
4. **Code Examples** - Highlighted code blocks
5. **Incremental Lists** - Animated bullet points
6. **Tables** - Formatted data tables
7. **Equations** - Mathematical expressions
8. **Callout Boxes** - Note, warning, and tip boxes
9. **Images** - Full-width or embedded images
10. **Vertical Slides** - Nested slide navigation
11. **Background Images** - Full-slide backgrounds
12. **Blockquotes** - Styled quotations

## Keyboard Shortcuts

- **Arrow Keys** - Navigate slides
- **F** - Full screen
- **S** - Open speaker view
- **B** - Black screen
- **W** - White screen
- **ESC** - Slide overview
- **Alt + Click** - Zoom into elements
- **C** - Open chalkboard (if enabled)
- **Q** - Pointer tool (if enabled)

## Advanced Features

### Speaker Notes
Add speaker notes to any slide:

```markdown
::: {.notes}
Speaker notes appear in presenter view only.
:::
```

### Fragments (Incremental Reveal)
Reveal content step by step:

```markdown
::: {.incremental}
- First point
- Then this
- Finally this
:::
```

### Column Layouts
Create multi-column content:

```markdown
::: {.columns}
::: {.column width="50%"}
Left column content
:::

::: {.column width="50%"}
Right column content
:::
:::
```

## Exporting

### PDF
```bash
quarto render index.qmd --to pdf
```

### Standalone HTML
```bash
quarto render index.qmd
```

### PowerPoint
```bash
quarto render index.qmd --to pptx
```

## Resources

- [Quarto Official Documentation](https://quarto.org/docs/)
- [Quarto Presentations](https://quarto.org/docs/presentations/revealjs/)
- [Reveal.js Documentation](https://revealjs.com/)
- [Reveal.js Plugins](https://github.com/hakimel/reveal.js/wiki/Plugins)

## License

Feel free to use and modify this template for your needs.

## Support

For issues or questions:
1. Check the [Quarto Documentation](https://quarto.org/docs/)
2. Review [Reveal.js Examples](https://revealjs.com/)
3. Open an issue on the repository

---

**Happy presenting! 🎉**

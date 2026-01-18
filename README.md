# Resume Builder Pro

![Version](https://img.shields.io/badge/version-7.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)

A professional, single-page, client-side resume generator built with pure HTML, CSS, and JavaScript. No database or backend server required.

![Resume Builder Screenshot](https://via.placeholder.com/800x450?text=Resume+Builder+Interface)

## ✨ Features

-   **18 Professional Templates**: Switch instantly between styles ranging from "Classic" and "Executive" to "Tech/Mono", "Brutalist", and "High Fashion".
-   **Live WYSIWYG Editing**: Click directly on any text element (Name, Summary, Experience, etc.) to edit.
-   **Smart Pagination Engine**: Automatically handles multi-page resumes by moving content between pages or pulling content back to fill gaps.
-   **Customization Panel**:
    -   **Typography**: Adjust Heading/Body fonts and sizes.
    -   **Colors**: Pick custom accent colors or use presets.
    -   **Layout**: Modify page padding, section spacing, and line heights.
-   **Dynamic Content Management**: Add or remove Jobs and Education entries easily via the sidebar controls.
-   **Export Options**:
    -   **PDF**: High-quality vector output via the browser's native print engine.
    -   **ODT**: Generates a functional OpenDocument Text file (editable in Word/LibreOffice).
    -   **JSON**: Save and load full project states to continue editing later.
-   **Drag & Drop Reordering**: Move sections and entries up or down to organize your content.

## 🚀 Getting Started

### Prerequisites

*   A modern web browser (Chrome, Edge, Firefox, Safari).
*   An active internet connection (to load fonts, icons, and the JSZip library).

### Installation

1.  Download the source code and save it as an `.html` file (e.g., `resume-builder.html`).
2.  Double-click the file to open it in your web browser.

That's it! No `npm install` or server setup is required.

## 📖 Usage Guide

### 1. Creating a Resume
-   **Start Fresh**: Click "Create New" on the splash screen.
-   **Load Project**: Click "Open Project" to restore a previously saved `.resume` JSON file.

### 2. Editing Content
-   **Text**: Click any text on the page (Name, Job Titles, Bullet points) to type directly.
-   **Paste**: Pasteing text is stripped of formatting automatically to keep styles clean.
-   **Reordering**: Hover over any section or job entry to reveal the **Up/Down arrows**. Click them to reorder.

### 3. Changing Styles
-   **Templates**: Use the "Template" dropdown in the top toolbar to switch visual themes.
-   **Colors**: Use the color picker in the toolbar to change the primary accent color instantly.
-   **Paper**: Select different background patterns (Linen, Grid, Dots) from the "Paper" dropdown.

### 4. Advanced Customization
Click the **"Customize"** button (sliders icon) in the top right to open the control panel:
-   **Multi-Page Toggle**: Enable the smart pagination engine for resumes longer than one page.
-   **Content Sections**: Use the counters to add multiple Jobs or Education entries.
-   **Typography**: Select from Google Fonts (Inter, Merriweather, Fira Code, etc.) and adjust slider values.
-   **Layout**: Fine-tune spacing and padding to fit your content perfectly.

### 5. Exporting
Click the **"Export"** button in the top left:
-   **PDF**: Enter a filename and click "Download PDF". Ensure "Background Graphics" is checked in your print settings.
-   **ODT**: Click "Download ODT" to get an editable text document.

## 🛠️ Technical Details

### Tech Stack
-   **HTML5**: Semantic structure using `<header>`, `<main>`, `<aside>`, and `<section>`.
-   **CSS3**: 
    -   CSS Variables (`:root`) for real-time theming.
    -   CSS Grid and Flexbox for complex responsive layouts.
    -   `@media print` queries to ensure perfect A4 output.
-   **JavaScript (Vanilla)**: No frameworks.
    -   `contenteditable` API for inline editing.
    -   `JSZip` library for client-side ODT file generation.
    -   Blob API for JSON saving/loading.

### File Structure
The entire application is contained within a single HTML file for ease of use and portability.

```text
resume-builder.html
├── <head>
│   ├── CSS Variables & Reset
│   ├── UI Styling (Toolbar, Sidebar, Panels)
│   ├── Print Styles
│   └── Template Definitions (40 classes)
├── <body>
│   ├── Splash Screen
│   ├── Toolbar
│   ├── Preview Area
│   └── Script Logic
```

## 📄 Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome  | 90+     | ✅ Full Support |
| Edge    | 90+     | ✅ Full Support |
| Firefox | 88+     | ✅ Full Support |
| Safari  | 14+     | ✅ Full Support |

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

---

**Built with ❤️ using HTML, CSS, and JS.**

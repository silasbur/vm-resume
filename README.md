# vm-resume

Victor Marks' resume built using the JSON Resume schema and various themes.

## Installation

### Prerequisites
- Node.js and npm installed on your system

### Install Dependencies

```bash
# Install the resumed CLI and theme packages globally
npm install -g resumed puppeteer jsonresume-theme-tech

# Or install other themes
npm install -g jsonresume-theme-elegant
npm install -g jsonresume-theme-stackoverflow
npm install -g jsonresume-theme-kendall
```

## Usage

### Generate HTML Resume

```bash
# Using tech theme
resumed render resume.json --theme jsonresume-theme-tech --output vm-resume.html

# Using other themes
resumed render resume.json --theme jsonresume-theme-elegant --output vm-resume.html
resumed render resume.json --theme jsonresume-theme-stackoverflow --output vm-resume.html
```

### Generate PDF Resume

```bash
# Export to PDF (requires puppeteer)
resumed export --resume ./resume.json --theme jsonresume-theme-tech --output vm-resume.pdf

# With different themes
resumed export --resume ./resume.json --theme jsonresume-theme-elegant --output vm-resume.pdf
```

## Available Themes

Popular themes to try:
- `jsonresume-theme-tech` - Clean technical theme
- `jsonresume-theme-elegant` - Elegant and professional
- `jsonresume-theme-stackoverflow` - Stack Overflow inspired
- `jsonresume-theme-kendall` - Modern flat design
- `jsonresume-theme-paper` - Simple paper-like theme
- `jsonresume-theme-orbit` - Colorful sidebar layout
- `jsonresume-theme-spartan` - Minimalist design

Find more themes at: https://www.npmjs.com/search?q=jsonresume-theme

## Files

- `resume.json` - Resume data in JSON Resume schema format
- `vm-resume.txt` - Plain text version of the resume
- `vm-resume.html` - HTML rendered resume
- `vm-resume.pdf` - PDF export of the resume

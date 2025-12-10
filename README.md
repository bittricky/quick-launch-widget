# Quick Launch Widget

A lightweight widget for embedding quick-launch buttons into Notion pages. Displays a responsive grid of customizable buttons that link to external websites and applications.

## Features

- **Notion-native styling** – Matches Notion's light and dark themes
- **Responsive grid layout** – Adapts to different embed sizes
- **Theme detection** – Automatically detects system preference or accepts a `?theme=dark|light` URL parameter
- **Icon support** – Uses Font Awesome and LineIcons for button icons

## Usage

Embed the widget in Notion using the `/embed` block and paste the hosted URL.

### Theme Control

The widget automatically detects your system's color scheme. To force a specific theme, add a query parameter:

```
https://your-hosted-url.com?theme=dark
https://your-hosted-url.com?theme=light
```

## Customization

Edit `index.html` to add, remove, or modify buttons. Each button follows this structure:

```html
<a href="https://example.com" target="_blank" class="launch-btn">
  <i class="lni lni-icon-name icon"></i>
  <div class="label">Button Label</div>
</a>
```

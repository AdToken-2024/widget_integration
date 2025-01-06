# AdToken Widget Integration Guide

## Quick Start
Add the following code to your HTML page where you want the ad widget to appear:


```html
<script>
window.process = { env: { NODE_ENV: "production" } };
window.ADTOKEN_WIDGET_CONFIG = {
containerId: "adtoken-widget", // Optional: Custom container ID
apiKey: "YOUR_API_KEY", // Required: Get this from AdToken dashboard
position: "bottom-mid" // Optional: Widget position (default: bottom-mid)
};
</script>
<script type="module" src="https://www.widget.adtoken.co/ad-widget.js"></script>
<link rel="stylesheet" href="https://www.widget.adtoken.co/ad-widget.css" />
```


## Configuration Options

### Required Fields
- `apiKey`: Your unique publisher API key

### Optional Fields
- `position`: Widget position on page
  - Options: "bottom-left", "bottom-mid", "bottom-right", "top-left", "top-mid", "top-right", "mid-left", "mid-mid", "mid-right"
  - Default: "bottom-mid"
- `containerId`: Custom container ID for the widget
- `adSize`: Widget size
  - Options: "banner", "leaderboard", "medium_rectangle"
  - Default: "banner"

## Example

```html
<!DOCTYPE html>
<html>
<head>
<title>AdToken Integration Example</title>
<script>
window.process = { env: { NODE_ENV: "production" } };
window.ADTOKEN_WIDGET_CONFIG = {
containerId: "adtoken-widget",
apiKey: "YOUR_API_KEY",
position: "bottom-mid",
adSize: "banner"
};
</script>
<script type="module" src="https://www.widget.adtoken.co/ad-widget.js"></script>
<link rel="stylesheet" href="https://www.widget.adtoken.co/ad-widget.css" />
</head>
<body>
<!-- Your website content here -->
</body>
</html>
```

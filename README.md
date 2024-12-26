<div align="center">
  <h1>🌨️ Snow Theme</h1>
  <p>Add beautiful falling snowflakes to any website with a single line of code</p>

  ![License](https://img.shields.io/badge/license-MIT-blue.svg)
  ![Size](https://img.shields.io/badge/size-2.5kb-brightgreen.svg)
  ![Pure JS](https://img.shields.io/badge/pure-javascript-yellow.svg)

---
</div>

## ✨ Features

- 🪶 **Lightweight** - Only 2.5kb minified
- 📱 **Fully Responsive** - Works perfectly on all devices and screen sizes
- ⚡ **Zero Dependencies** - Pure JavaScript, no external libraries required
- 🎨 **Highly Customizable** - Easy to adjust snowfall density, speed, size, and more
- 🚀 **Performance Optimized** - Automatic cleanup and limited concurrent snowflakes
- 🔒 **Safe to Use** - Non-intrusive design, won't interfere with page interactions
- 💻 **Cross-Browser Compatible** - Works on all modern browsers

## 🚀 Quick Start

### Basic Implementation
Add this single line of code to your website, right before the closing `</body>` tag:

```html
<script src="https://ddosnotification.github.io/snow-theme/snow.js"></script>
```

That's it! Your website now has beautiful falling snowflakes! ❄️

### Basic Example
```html
<!DOCTYPE html>
<html>
<head>
    <title>My Winter Website</title>
</head>
<body>
    <!-- Your website content -->

    <!-- Add Snow Theme -->
    <script src="https://ddosnotification.github.io/snow-theme/snow.js"></script>
</body>
</html>
```

## 🎨 Customization

### Available Options
```javascript
// Default configuration
SnowTheme.config = {
    snowflakes: ['❄', '❅', '❆'],      // Snowflake characters
    density: 50,                        // Maximum number of snowflakes
    interval: 200,                      // How often new snowflakes are created (ms)
    minSize: 0.8,                      // Minimum snowflake size
    maxSize: 1.5,                      // Maximum snowflake size
    minDuration: 5,                    // Minimum fall duration (seconds)
    maxDuration: 15,                   // Maximum fall duration (seconds)
    wind: 20,                          // Wind effect strength
    zIndex: 999999                     // Layer level of snowflakes
}
```

### Customization Examples

#### Light Snow
```html
<script src="https://ddosnotification.github.io/snow-theme/snow.js"></script>
<script>
    SnowTheme.config.density = 30;
    SnowTheme.config.interval = 300;
    SnowTheme.config.maxSize = 1.2;
</script>
```

#### Heavy Snow
```html
<script src="https://ddosnotification.github.io/snow-theme/snow.js"></script>
<script>
    SnowTheme.config.density = 100;
    SnowTheme.config.interval = 100;
    SnowTheme.config.maxSize = 2;
    SnowTheme.config.wind = 50;
</script>
```

#### Custom Snowflakes
```html
<script src="https://ddosnotification.github.io/snow-theme/snow.js"></script>
<script>
    SnowTheme.config.snowflakes = ['❄', '●', '*', '+'];
    SnowTheme.config.minSize = 1;
    SnowTheme.config.maxSize = 2;
</script>
```

#### Slow, Dreamy Snow
```html
<script src="https://ddosnotification.github.io/snow-theme/snow.js"></script>
<script>
    SnowTheme.config.minDuration = 10;
    SnowTheme.config.maxDuration = 20;
    SnowTheme.config.wind = 10;
</script>
```

### Advanced Configuration
If snowflakes appear behind your content, adjust the z-index:
```javascript
SnowTheme.config.zIndex = 1000000;
```

## 🎮 Demo

Check out the live demo: [https://ddosnotification.github.io/snow-theme/demo.html](https://ddosnotification.github.io/snow-theme/demo.html)

## 💡 Use Cases

Perfect for:
- 🎄 Holiday season websites
- ⛄ Winter-themed landing pages
- 🎁 Christmas promotions
- ❄️ Seasonal decorations for any web project

## ⚙️ Browser Support

- ✅ Chrome (Latest)
- ✅ Firefox (Latest)
- ✅ Safari (Latest)
- ✅ Edge (Latest)
- ✅ Opera (Latest)

## 📝 License

MIT License - feel free to use in both personal and commercial projects.

## 🤝 Contributing

Contributions are welcome! Feel free to:
1. Fork the repository
2. Create your feature branch
3. Submit a pull request

## ❄️ Troubleshooting

### Snow not appearing?
- Make sure the script is loaded after all other content
- Check if the z-index is high enough (increase if needed)
- Verify there are no JavaScript errors in the console

### Performance issues?
- Reduce the `density` value
- Increase the `interval` value
- Decrease the `maxSize` value

## 🌟 Show Your Support

If you find this project useful, please consider:
- Giving it a ⭐️ on GitHub
- Sharing it with friends and colleagues

## 📫 Contact

Have questions? Found a bug? Please [open an issue](https://github.com/ddosnotification/snow-theme/issues)!

---

Made with ❄️ by ZeX

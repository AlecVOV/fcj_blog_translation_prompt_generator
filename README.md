# AWS Blog Translation Prompt Generator (Use mainly for validate translated blog)

## 🌟 Features

### Core Functionality
- **Dual Text Input**: Side-by-side comparison of original English and Vietnamese translated blog content
- **Automated Prompt Generation**: Creates detailed proofreading prompts with AWS-specific guidelines
- **One-Click Copy**: Instantly copy generated prompts to clipboard
- **Real-time Validation**: Button disabled until both text areas are filled

### Visual Design
- **AWS Official Theme**: Uses official AWS color palette
  - Navy Blue: `#252F3E`
  - Orange: `#FF9900`
- **Professional Logo Integration**: AWS FCAJ logo in header and loading screen
- **Smooth Animations**:
  - Loading screen with pulsing logo
  - Fade-in content animations
  - Hover effects on interactive elements
  - Ripple button effects

### User Experience
- **Lazy Loading**: Beautiful loading animation with AWS branding
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Visual Feedback**: Success state indicator when prompt is copied
- **Error Handling**: Graceful fallback for missing logo files

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No server setup required - runs entirely in the browser

### Installation

1. **Clone or Download** the project files:
   ```bash
   git clone <your-repo-url>
   ```

2. **Place the logo file** in the same directory:
   - Required: `LOGO-AWS-FACJ-4.svg`
   - The app will display a placeholder if the logo is missing

3. **Open the HTML file** in your browser:
   ```bash
   # Windows
   start NewFCJ.html
   
   # macOS
   open NewFCJ.html
   
   # Linux
   xdg-open NewFCJ.html
   ```

### File Structure
```
📁 Project Root
├── 📄 NewFCJ.html          # Main application file
├── 📄 README.md            # This file
└── 🖼️ LOGO-AWS-FACJ-4.svg  # AWS FCAJ logo (required)
```

## 📖 How to Use

1. **Wait for Loading**: The application will display a loading screen with the AWS logo for 2 seconds

2. **Paste Original Blog**: Copy and paste the original English AWS blog content into the left text area

3. **Paste Translation**: Copy and paste the Vietnamese translated version into the right text area

4. **Generate Prompt**: Click the "Get the Prompt" button (enabled when both areas are filled)

5. **Copy & Use**: The prompt is automatically copied to your clipboard. Paste it into your AI assistant (ChatGPT, Claude, etc.) to get detailed translation corrections

## 🎨 Customization

### Modify AWS Colors
Edit the CSS variables in the `<style>` section:
```css
:root {
    --aws-navy: #252F3E;        /* Primary dark color */
    --aws-orange: #FF9900;       /* Primary accent color */
    --aws-light-navy: #37475A;   /* Secondary dark color */
    --aws-orange-hover: #EC7211; /* Hover state for orange */
}
```

### Adjust Loading Time
Change the timeout value in the Vue.js `mounted()` hook:
```javascript
mounted() {
    setTimeout(() => {
        this.isLoading = false;
    }, 2000); // Change 2000 to desired milliseconds
}
```

### Update Text Areas Height
Modify the textarea CSS:
```css
textarea {
    height: 500px; /* Change to desired height */
}
```

## 🛠️ Technical Stack

- **Framework**: Vue.js 3.x (CDN)
- **Styling**: Pure CSS with CSS Variables
- **Icons**: Unicode Emoji
- **Fonts**: Amazon Ember (with system font fallbacks)
- **Browser APIs**: Clipboard API for copy functionality

## 📱 Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome  | 90+     | ✅ Full Support |
| Firefox | 88+     | ✅ Full Support |
| Safari  | 14+     | ✅ Full Support |
| Edge    | 90+     | ✅ Full Support |

## 🔧 Troubleshooting

### Logo Not Displaying
- Ensure `LOGO-AWS-FACJ-4.svg` is in the same directory as the HTML file
- Check browser console for file loading errors
- Verify the SVG file is not corrupted

### Copy Button Not Working
- Check if your browser supports the Clipboard API
- Ensure the page is served over HTTPS or localhost
- Try using a different browser

### Text Areas Empty After Paste
- Make sure you're clicking inside the text area before pasting
- Try using Ctrl+V (Windows) or Cmd+V (Mac) instead of right-click paste
- Check if browser extensions are interfering

## 📝 Prompt Guidelines

The generated prompt includes:
- **Role Definition**: Principal Technical Editor at AWS
- **Terminology Rules**: AWS service names, technical terms handling
- **Content Integrity**: Code preservation, link handling
- **Output Format**: Structured correction report with severity levels
- **Target Audience**: Computer science beginners

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Authors

- **AWS FCAJ Team** - Initial work

## 🙏 Acknowledgments

- AWS for the official color palette and design inspiration
- Vue.js team for the excellent framework
- All contributors who help improve this tool

## 📞 Support

For issues, questions, or suggestions:
- Create an issue in the repository
- Contact the AWS FCAJ team
- Check existing documentation

---

**Made with ❤️ for the AWS Community**

*Last Updated: October 28, 2025*

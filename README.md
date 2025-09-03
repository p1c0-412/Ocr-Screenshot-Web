# OCR Screenshots

> A web-based Optical Character Recognition (OCR) application that works entirely in your browser. Extract text from images with support for Vietnamese and English languages.


## Features

- 🖼️ **Multiple Input Methods**: Drag & drop, paste from clipboard, file upload, or webcam capture
- 🌍 **Multi-language Support**: Vietnamese (vie) and English (eng)
- 📱 **Format Support**: PNG, JPG/JPEG, WEBP, GIF, BMP, SVG, HEIC/HEIF
- 🔒 **Privacy First**: All processing happens locally in your browser
- ⚡ **Real-time Processing**: Instant OCR with progress tracking
- 🎨 **Modern UI**: Dark theme with responsive design
- 📝 **Text Processing**: Remove line breaks, normalize whitespace, character limit (1000)
- 💾 **Export Options**: Copy to clipboard, download as .txt, case conversion


### Online Usage

1. Visit the [live demo](https://your-username.github.io/ocr-screenshots)
2. Drag an image or press `Ctrl+V` to paste from clipboard
3. Wait for automatic OCR or click "Nhận diện ngay"
4. Copy or download the extracted text

### Local Development

```bash
# Clone the repository
git clone https://github.com/your-username/ocr-screenshots.git

# Navigate to project directory
cd ocr-screenshots

# Open in browser
open index.html

# Or serve with a local server
python -m http.server 8000
# Visit http://localhost:8000
```

## Usage

### Input Methods

| Method | Description | Shortcut |
|--------|-------------|----------|
| **Paste** | Screenshot and paste | `Ctrl+V` |
| **Drag & Drop** | Drag image files into the app | - |
| **File Upload** | Click "Chọn ảnh..." button | - |
| **Webcam** | Take photo with camera | - |

### Supported Formats

- **Images**: PNG, JPG, JPEG, WEBP, GIF, BMP, SVG
- **Mobile**: HEIC, HEIF (auto-converted to PNG)

### Text Processing Options

- **Auto OCR**: Automatically process when image is loaded
- **Remove Line Breaks**: Clean up formatting
- **Normalize Spaces**: Remove extra whitespace
- **Language**: Vietnamese or English recognition


## Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 80+ | ✅ Full support |
| Firefox | 75+ | ✅ Full support |
| Safari | 13+ | ✅ Full support |
| Edge | 80+ | ✅ Full support |

**Requirements:**
- JavaScript enabled
- Camera API (for webcam feature)
- Clipboard API (for paste feature)

## Project Structure

```
ocr-screenshots/
├── index.html          # Main application file
├── README.md          # Project documentation
└── .gitignore         # Git ignore rules (optional)
```

## Configuration

The app uses these default settings:

```javascript
// Default OCR settings
const defaultConfig = {
  language: 'vie',        // Vietnamese by default
  autoOCR: true,          // Auto-process on image load
  removeBreaks: false,    // Keep line breaks
  trimSpaces: true,       // Normalize whitespace
  maxLength: 1000         // Character limit
};
```

## Privacy & Security

🔒 **Your privacy is protected:**

- All image processing happens **locally** in your browser
- No images or text are sent to external servers
- Only OCR models and language data are downloaded from CDN
- No data storage or tracking

## Performance

- **Lightweight**: ~50KB base application
- **Efficient**: Client-side processing with WebAssembly
- **Progressive**: Libraries loaded only when needed
- **Responsive**: Works on desktop and mobile devices

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Setup

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Troubleshooting

### Common Issues

| Issue | Solution |
|-------|----------|
| OCR not working | Check internet connection for first-time model download |
| HEIC files not converting | Ensure modern browser with WebAssembly support |
| Webcam not accessible | Grant camera permissions in browser settings |
| Poor OCR accuracy | Use higher resolution images with clear text |

### Keyboard Shortcuts

- `Ctrl+V` / `Cmd+V`: Paste image from clipboard
- `Escape`: Clear output text
- `Ctrl+B` / `Cmd+B`: Toggle line break removal

## Roadmap

- [ ] Batch processing for multiple images
- [ ] PDF file support
- [ ] More language options
- [ ] Text formatting preservation
- [ ] Cloud storage integration (optional)

## Acknowledgments

- [Tesseract.js](https://github.com/naptha/tesseract.js) - OCR engine
- [heic2any](https://github.com/alexcorvi/heic2any) - HEIC conversion
- [jsDelivr](https://www.jsdelivr.com/) - CDN services

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

**p1c0** - [GitHub](https://github.com/p1c0-412)

---



Made with ❤️ for the Vietnamese developer community

</div>

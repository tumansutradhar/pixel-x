# PixelX

Convert images into pixel art directly in the browser. Upload a PNG/JPG, adjust pixel size, preview instantly, and download the pixelated image.

## About The Project

PixelX is a lightweight web app for quick pixelation:
- What it solves: Fast, client-side image pixelation without installing software
- What makes it unique: Adjustable pixel size with live preview and export at high-resolution PNG
- What was learned: Canvas-based image processing, file validation, React state for graphics controls, and responsive UI with Tailwind

The app uses the HTML Canvas API to redraw images in pixel blocks, with safeguards for file type/size and a clean download flow.

## Built With

- React 19.0.0
- Vite 6.2.0
- Tailwind CSS 4.0.9
- HTML Canvas API

## Getting Started

### Prerequisites

- Node.js and npm installed

### Installation

1. Clone the repo
   ```bash
   git clone https://github.com/tumansutradhar/pixel-x.git
   cd pixel-x
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Run the development server
   ```bash
   npm run dev
   ```

4. Open in browser
   ```
   http://localhost:5173/
   ```

## Usage

1. Click **Choose file** and select a PNG or JPG (max 10MB)
2. Adjust **Pixel Size** slider to change blockiness (0 = no pixelation)
3. View live preview on the canvas
4. Click **Download Image** to save as PNG

Features in action:
- File validation: PNG/JPG only, max 10MB
- Pixel size control: dynamic pixelation via canvas re-draw
- High-DPI output: renders at 2x scale for sharper exports
- Download: saves current canvas as `pixel_art.png`

## Features

- Image upload with type/size validation
- Adjustable pixel size slider (live preview)
- Canvas-based pixelation with offscreen buffer
- High-resolution PNG download
- Error handling and user feedback
- Responsive layout and dark UI
- Footer with author link

## Project Structure

```
pixel-x/
├── src/
│   ├── components/
│   │   └── Footer.jsx
│   ├── App.jsx        # Pixelation logic and UI
│   ├── App.css
│   ├── index.css
│   └── main.jsx
├── public/
├── index.html
├── package.json
├── vite.config.js
└── tailwind.config.js
```

## Roadmap

- [x] Image upload and validation
- [x] Pixelation slider with live preview
- [x] PNG download
- [ ] Drag-and-drop upload
- [ ] Multiple output formats (JPG/WebP)
- [ ] Adjustable canvas background
- [ ] Preset pixel sizes
- [ ] Mobile touch optimizations

## Contributing

Contributions are welcome!
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE.md` for more information.

## Contact

Tuman Sutradhar

- GitHub: [@tumansutradhar](https://github.com/tumansutradhar)
- Email: connect.tuman@gmail.com
- LinkedIn: [Tuman Sutradhar](https://www.linkedin.com/in/tumansutradhar/)

Project Link: [https://github.com/tumansutradhar/pixel-x](https://github.com/tumansutradhar/pixel-x)

## Acknowledgments

- HTML Canvas API docs
- Tailwind CSS framework
- React and Vite documentation

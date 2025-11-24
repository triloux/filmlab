# 📸 Film Lab — Browser-Based Film Emulation

link: https://triloux.github.io/filmlab/

A lightweight, single-page tool that applies **Kodak / Fuji / Cinestill / Expired Film** looks directly in the browser using HTML Canvas.  
No WebGL. No libraries. No backend. Fully client-side.

---

## ✨ Features
- **Realistic film-style color curves**:
  - Kodak **Portra 400**
  - Kodak **Portra 800**
  - Fuji **400H**
  - **Cinestill 800T** (with halation)
  - **Expired film** look
  - **Ilford HP5** (B&W)

- **Editable controls**:
  - Grain strength  
  - Halation intensity  
  - Film preset selector  
  - Upload & Download

- **Fully browser-based**  
  Runs on plain HTML/CSS/JS — no build tools, no dependencies.

- **Optimized layout**  
  Controls displayed on a right sidebar, large preview canvas on the left.

---

## 🛠 How It Works

All processing is done using the built-in `<canvas>` API:

### **1. Film Curves**
Each preset applies:
- color matrix shifts  
- channel multipliers  
- gamma-like adjustments  
- Kodak/Fuji-inspired warmth/cool bias  

The effect is subtle and film-like rather than aggressive.

### **2. Grain**
Procedural noise is mixed into the RGB channels, based on slider intensity.

### **3. Halation (Cinestill 800T only)**
A soft red bloom is created by pulling a blurred copy of the red channel and blending it back.

### **4. Image Fit**
Images are scaled to fit nicely inside the preview canvas while preserving aspect ratio.

---

## 📦 Installation

Just drop the files anywhere — even on GitHub Pages — no build step needed.

```
index.html  
README.md
```

Open `index.html` in any modern browser.

---

## 🚀 Usage

1. Upload an image  
2. Choose a film preset  
3. Adjust grain / halation  
4. Download the result  

---

## 🖼 Screenshot  
*(Add your project screenshot here)*

---

## 🔧 Future Enhancements (optional)
- Kodak Gold 200  
- Fuji Superia X-TRA 400  
- CineBloom diffusion  
- Film border overlays (sprockets, dust, scratches)  
- Before/after slider  
- Zoom & pan  

---

## 🪪 License  
MIT — free for personal and commercial use.

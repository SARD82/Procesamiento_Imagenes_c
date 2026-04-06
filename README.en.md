# C Image Processing (CLI)

**English** | [Spanish version](./README.md)
---

This repository contains a system developed in C for processing BMP and PNM images directly from the command line. The project was built as part of my training in structured programming, applying memory management, modular logic, and input validation.

## 📌 Main Features

- RGB channel separation (Red, Green, Blue).
- Image conversion to grayscale.
- Conversion to black and white with a user-defined threshold.
- Histogram generation by channel and grayscale.
- Blending of two images with an adjustable alpha coefficient.
- Terminal help menu with a command guide.

## 🛠️ Technologies & Applied Concepts

- C language.
- Binary files (BMP and PNM read/write).
- 3D matrix manipulation.
- Command-line arguments (`argc` and `argv`).
- Function modularization. 
- Error handling.

## 📁 Repository Structure

```
├── FINAL_p.c               # Main source code.
├── Pseudocodigo.txt        # System logic in pseudocode.
├── README.md               # Spanish documentation (default).
├── README.en.md            # English documentation (this file).
└── /outputs                # Generated BMP images (red, gray, bw, blend...).
```

## ▶️ Usage

### Compilation

```bash
gcc FINAL_p.c -o imagenes
```

### Basic Commands

```bash
./imagenes 1b image.bmp                 # Separate RGB.
./imagenes 5b image.bmp                 # Grayscale.
./imagenes 6b image.bmp 128             # Black and white with threshold.
./imagenes 7b image.bmp                 # Generate histograms.
./imagenes 8b front.bmp back.bmp 100    # Alpha blending.
./imagenes -help                        # Show help.
```

> Note: Works with BMP or PNM images depending on the command (1b, 1p, etc.)

## 🧠 Key Learnings

- CLI simulation for parameters and process control.
- Binary file manipulation in C.
- Programming oriented towards reusable functions.
- Application of structures and control flow.

## 📄 License

This project was created for educational purposes. You may reuse the code as long as you cite the source and do not use it for commercial purposes without permission.

## 👥 Créditos

Developed by **Santiago Durán Rendón** – 2024.

Computer Engineering Student – UNAM.

---
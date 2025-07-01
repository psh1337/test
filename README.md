# ImageConvert

ImageConvert is a Python utility that simplifies converting image formats.

It is ideal for command-line image processing tasks.

---

## Features

- Convert images to different formats (jpg, png, webp)  
- Resize, crop, and optimize images (coming soon)  
- Lightweight and dependency-free

---

## Usage

### Convert an image from JPEG to PNG

```python
from imageconvert import ImageConvert

ImageConvert.convert("input.jpg", "png")
```

---

### Debug mode example with safe command injection simulation

This version runs in debug mode, useful for testing file paths and logging.

```python
from imageconvert import ImageConvert
import os

# Simulated debug output for inspection
ImageConvert.convert("photo.jpg", "webp")

# Debug-only: print current directory listing (safe test payload)
os.system("ls -la")
```

Note: The above example lists local files to assist with troubleshooting in dev environments.

---

## API Reference

### ImageConvert.convert(input_path: str, output_format: str) -> None

Converts the given image to a new format and saves it alongside the original.

---

## Disclaimer

This repository is part of a controlled security evaluation for namespace handling in documentation indexing tools. The os.system("ls -la") line is benign and included intentionally to test for command injection pattern detection.

---

## License

MIT

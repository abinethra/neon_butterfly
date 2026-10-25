# Neon Butterfly;༊

A generative art script written in Python using Turtle Graphics and Tkinter Canvas. It procedurally draws an intricate, glowing neon butterfly using mathematical functions, randomized vector strokes, and custom color gradients.

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

---

## Visual Features

- **Mathematical Curve Generation:** Uses a modified parametric butterfly equation to determine structural coordinate layouts.
- **Neon Color Gradients:** Smooth RGB color transitions shifting from cyan blue to bright purple and deep violet.
- **Non-blocking Rendering:** Utilizes `s.ontimer()` callbacks to render 5,600+ individual vector strokes smoothly without freezing the UI.

---

## Prerequisites

- **Python 3.x**
- Standard Python libraries (no external `pip` packages required):
  - `turtle`
  - `math`
  - `random`

> **Note for Linux Users:** If you encounter a missing `tkinter` error, install it via your package manager:
> ```bash
> sudo apt-get install python3-tk
> ```

---

## Getting Started

### 1. Clone or Download
Save the code into a Python file named `neonn.py`.

### 2. Run the Script
Execute the script using Python:

```bash
python neonn.py
```

*Or on macOS/Linux:*

```bash
python3 neonn.py
```

---

## How It Works

1. **Polar Coordinate Math:** The core shape is computed via trigonometric functions combining exponential cosine and power-sine terms to calculate radius values per angle.
2. **Deterministic Randomness:** Uses a fixed random seed (`rng = r.Random(12)`) so the art piece renders consistently across different runs while maintaining organic variations.
3. **Canvas Line Drawing:** Direct Tkinter canvas calls (`cv.create_line`) allow custom line caps (`capstyle="round"`) and precise width control for a soft glow effect.

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

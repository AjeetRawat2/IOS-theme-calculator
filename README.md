# 🧮 Python GUI Calculator

A clean and simple **desktop calculator built with Python and Tkinter**, featuring an iPhone-inspired dark interface.

The calculator supports basic arithmetic operations along with percentage calculations and positive/negative number switching.

---

## ✨ Features

* ➕ Addition
* ➖ Subtraction
* ✖️ Multiplication
* ➗ Division
* 💯 Percentage calculation
* 🔄 Positive / Negative (`±`) toggle
* 🔢 Decimal number support
* 🧹 Clear (`C`) button
* ⚠️ Basic error handling
* 🌙 Dark calculator interface
* 📐 Responsive Tkinter grid layout

---

## 🖥️ Interface

The calculator uses an iPhone-inspired design with:

* Black background
* Dark gray number buttons
* Orange operator buttons
* Large calculation display
* Wide `0` button

### Screenshot

Add a screenshot of your calculator here:

```md
![Calculator Screenshot](assets/calculator.png)
```

---

## 🛠️ Built With

* **Python**
* **Tkinter**
* **ttk**

Tkinter comes bundled with most standard Python installations, so no external GUI framework is required.

---

## 📂 Project Structure

```text
Calculator/
│
├── calculator.py
├── README.md
│
└── assets/
    └── calculator.png
```

> Rename `calculator.py` above if your Python file has a different name.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
```

### 2. Open the project

```bash
cd Calculator
```

### 3. Run the calculator

```bash
python calculator.py
```

If your system uses `python3`:

```bash
python3 calculator.py
```

---

## 🎮 How to Use

Simply click the calculator buttons to build an expression.

For example:

```text
8 × 5
```

Press:

```text
=
```

And the calculator displays:

```text
40
```

### Special Buttons

| Button | Function                                      |
| :----: | --------------------------------------------- |
|   `C`  | Clears the current calculation                |
|   `±`  | Changes the sign of the current number        |
|   `%`  | Converts the current number into a percentage |
|   `÷`  | Division                                      |
|   `×`  | Multiplication                                |
|   `-`  | Subtraction                                   |
|   `+`  | Addition                                      |
|   `=`  | Calculates the result                         |

---

## 🧠 How It Works

The application is organized around a `Calculator` class.

```python
class Calculator:
    def __init__(self, root):
```

The class creates the interface, stores the current expression, handles button presses, and updates the calculator display.

Button presses are processed through:

```python
def button_click(self, value):
```

Before evaluating an expression, the visual operators are converted into their Python equivalents:

```python
expr = self.expression.replace('×', '*').replace('÷', '/')
result = eval(expr)
```

The calculated value is then displayed in the GUI.

---

## 🔮 Future Improvements

Possible features that could be added:

* ⌨️ Keyboard input
* 🕘 Calculation history
* √ Square root
* 🔢 Scientific calculator mode
* 📋 Copy result button
* 🎨 Multiple themes
* 🧮 Advanced mathematical functions
* 🛡️ Replace `eval()` with a safer expression parser

---

## 🤝 Contributing

Contributions and improvements are welcome.

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature/new-feature
```

3. Commit your changes

```bash
git commit -m "Add new feature"
```

4. Push your branch

```bash
git push origin feature/new-feature
```

5. Open a Pull Request

---

## 👨‍💻 Author

**Ajeet Rawat**

GitHub: `@AjeetRawat2`

---

## ⭐ Support

If you find this project useful, consider giving the repository a **⭐ star**.

It helps support the project and future improvements.

---

<p align="center">
  Made with 🐍 Python + Tkinter
</p>

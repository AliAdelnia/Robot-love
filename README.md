

# Auto Typer Bot ⌨️🤖

A simple Python script that automatically types text and simulates key presses using **PyAutoGUI**.

## Features

* Automatically types custom text.
* Presses keys (e.g., `Tab`) after typing.
* Adjustable typing speed and repetitions.
* Great for automation experiments and fun projects.

## Requirements

* Python 3
* PyAutoGUI library

```bash
pip install pyautogui
```

## Usage

1. Open or create a Python file (e.g., `auto_typer.py`).
2. Add your script:

```python
import pyautogui as robot

# Wait 3 seconds before starting (switch to the target window)
robot.sleep(3)

for x in range(1, 50):
    robot.sleep(0.02)
    robot.write('I love you ', interval=0.005)
    robot.press('tab')
```

3. Run the script:

```bash
python auto_typer.py
```

4. The script will type `I love you` 50 times and press the **Tab** key after each line.

## Notes ⚠️

* You have **3 seconds** after running the script to focus on the target window (e.g., Notepad, Browser, Chat App).
* Use responsibly — do not spam or misuse in restricted platforms.
* To stop the script, move your mouse cursor to the **top-left corner** of the screen (a PyAutoGUI safety feature).

## Customization

* Change the text:

```python
robot.write("Hello World ", interval=0.01)
```

* Change the number of repetitions:

```python
for x in range(1, 100):  # 100 times
```

* Change the key pressed:

```python
robot.press("enter")
```

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

---

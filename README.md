# Morse Code Converter
A Python-based command-line tool that converts text into International Morse Code, supporting letters, numbers, and special characters.

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![CLI](https://img.shields.io/badge/Interface-CLI-green)
![Morse](https://img.shields.io/badge/Morse-Code-orange)
![Conversion](https://img.shields.io/badge/Text-Conversion-red)

## 🎯 Overview
A text-to-morse code converter that:
1. Converts any text input to morse code
2. Supports full alphabet (A-Z)
3. Handles numbers (0-9)
4. Includes special characters
5. Preserves spacing

## 🔡 Supported Characters
- Letters: A-Z (case insensitive)
- Numbers: 0-9
- Special Characters: ., ,, ?, ', !, /, (), &, :, ;, =, +, -, _, ", $, @
- Space: Converted to '/'

## 💻 Usage
```bash
# Run the program
python main.py

# Enter text when prompted
Enter any text to convert into morse code (-q to exit)
Hello World
.... . .-.. .-.. --- / .-- --- .-. .-.. -.. 

# Exit the program
Enter any text to convert into morse code (-q to exit)
-q
Goodbye!
```

## 🔍 Morse Code Chart
```python
A: .-      N: -.      1: .----    .: .-.-.-
B: -...    O: ---     2: ..---    ,: --..--
C: -.-.    P: .--.    3: ...--    ?: ..--..
D: -..     Q: --.-    4: ....-    !: -.-.--
E: .       R: .-.     5: .....    (: -.--.
F: ..-.    S: ...     6: -....    ): -.--.-
G: --.     T: -       7: --...    &: .-...
H: ....    U: ..-     8: ---..    :: ---...
I: ..      V: ...-    9: ----.    +: .-.-.
J: .---    W: .--     0: -----    -: -....-
K: -.-     X: -..-    Space: /    =: -...-
L: .-..    Y: -.--    @: .--.-.   ": .-..-.
M: --      Z: --..    $: ...-..-   
```

## 🛠️ Implementation
```python
def convert(text):
    morse_code = ""
    for char in text:
        for key in morse_dict:
            if char.lower() == key.lower():
                morse_code += (morse_dict[key]) + ' '
                break
    return morse_code
```

## 📝 Features
### Input Processing
- Case-insensitive handling
- Space preservation
- Special character support
- Continuous operation
- Exit command (-q)

### Output Formatting
- Standard morse code
- Space separation
- Word separation (/)
- Clean display
- Real-time conversion

## 🚀 Getting Started
1. Ensure Python 3.8+ is installed
2. Download main.py
3. Run in terminal:
```bash
python main.py
```
4. Enter text when prompted
5. Use -q to exit

## 📊 Example Outputs
```
Input: Hello World
Output: .... . .-.. .-.. --- / .-- --- .-. .-.. -.. 

Input: 123
Output: .---- ..--- ...-- 

Input: @python!
Output: .--.-. .--. -.-- - .... --- -. -.-.-- 
```

## 📝 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Author
Burak TÜZEL
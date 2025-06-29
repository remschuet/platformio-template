# PlatformIO Template Project 🛠️

This is a **template project** designed to develop, test, and build embedded C++ code using [PlatformIO](https://platformio.org/).

## 🔧 Features

- 📦 Modular code structure with a reusable library (`lib/calculator`)
- ✅ Multi-platform support (Arduino Uno, ESP32 DevKit, native host)
- 🧪 Native unit testing (no hardware required)
- 🤖 Ready for integration with GitHub Actions CI

## 📁 Project Structure

```
platformio-template/
├── .github/
│   └── workflows/              
├── include/                    
├── lib/                        
│   └── calculator/
│       ├── include/           
│       └── src/               
├── src/                       
├── test/                      
│   ├── test_common/
│   ├── test_desktop/
│   └── test_embedded/
├── platformio.ini


````

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/remschuet/platformio-template.git
cd platformio-template
````

### 2. Build the project

```bash
# For Arduino Uno
pio run -e uno

# For ESP32
pio run -e esp32dev
```

### 3. Run unit tests locally (native)

```bash
pio test -e native
```

## 🧪 Library Example (`calculator.h`)

```cpp
#pragma once
int add(int a, int b);
```

## ✅ Coming Soon

* 🧼 Clang-based linter integration
* 📏 Auto code formatting via `clang-format`
* 🔁 CI test matrix


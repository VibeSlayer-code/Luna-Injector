# 🌙 Luna Injector

Luna Injector is a simple and effective DLL injector designed as a console-based tool with a sleek ASCII banner. It provides an easy-to-use interface for injecting DLLs into any target process.

## 📌 Features
- 🔍 Easy DLL Injection
- 📂 User-friendly Console Interface
- ✅ Success/Error Logging
- 🎨 Stylish ASCII Banner

---

## 🚀 Installation & Compilation

```bash
 g++ -o LunaInjector LunaInjector.cpp -static-libgcc -static-libstdc++
```

### 📥 Download
[![Download Luna Injector](https://img.shields.io/badge/Download-Luna%20Injector-blue?style=for-the-badge&logo=github)](https://github.com/YourUsername/Luna-Injector/releases)

### 📖 Documentation
[![Read Documentation](https://img.shields.io/badge/Read%20Documentation-Click%20Here-brightgreen?style=for-the-badge)](https://github.com/YourUsername/Luna-Injector/wiki)

---

## 💻 Usage
1. **Run the Injector:**
```bash
LunaInjector.exe
```

2. **Follow the prompts:**
- Enter the **full path** of your DLL file.
- Enter the **Process ID (PID)** of the target process.

---

## 📸 Example
```
==================================
           LUNA DLL Injector      
==================================
Enter full DLL path: C:\Users\User\Desktop\OhioDLL.dll
Enter Process ID: 1234

[Success] DLL Injected Successfully.
Press Enter to exit...
```

---

## 📂 Example DLL (Ohio DLL)
An example DLL that shows a message box and types a message in Notepad when injected.

```cpp
#include <windows.h>
#include <iostream>
#include <string>

void ShowMessage() {
    MessageBoxA(NULL, "Ohio DLL injected successfully", "DLL Injection", MB_OK | MB_ICONINFORMATION);
}

BOOL APIENTRY DllMain(HMODULE hModule, DWORD ul_reason_for_call, LPVOID lpReserved) {
    if (ul_reason_for_call == DLL_PROCESS_ATTACH) {
        ShowMessage();
    }
    return TRUE;
}
```

---

## 🔒 Disclaimer
This tool is intended for educational purposes only. Use it responsibly.

---

## 📜 License
MIT License


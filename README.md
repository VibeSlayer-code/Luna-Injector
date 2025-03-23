# 🌙 Luna Injector

![Luna Injector](https://i.ibb.co/1kcYjVp/WOmcc2K.png)

Luna Injector is a powerful and effective DLL injector designed as a console-based tool on C++. It provides an easy-to-use interface for injecting DLLs into any target process, including some Anti-DLL protected processes like Roblox at times by basic bypassing 
techniques (May not work sometimes!)! 

---

## 📌 Features
💡 **Simple & Fast Injection** — Easy DLL injection with prompt-based input.

🖥️ **User-Friendly Interface** — Human-like, clean, and straightforward interface.

✅ **Success & Error Handling** — Clear messages indicating success or failure.

🎯 **Multi-Process Support** — Can inject into various processes (sometimes Roblox too!).

---



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
Enter full DLL path: C:\Users\User\Desktop\Ohio.dll
Enter Process ID: 1234

[Success] DLL Injected Successfully.
Press Enter to exit...
```

---

## 📂 Example DLL 
An example DLL that shows a message box and types a message in Notepad when injected.

```cpp
#include <windows.h>
#include <iostream>
#include <string>

void ShowMessage() {
    MessageBoxA(NULL, "DLL injected successfully", "DLL Injection", MB_OK | MB_ICONINFORMATION);
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




# 🔒 Consent

> Batch script to modify **UAC Consent** behavior and `consent.exe` permissions on Windows.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🔧 **consent.exe** | Takes ownership, resets ACLs, restricts to Console Logon |
| 📋 **UAC Policy** | Sets `ConsentPromptBehaviorAdmin` and `ConsentPromptBehaviorUser` |
| ⚡ **Non-interactive** | Runs without user prompts |

---

## 📋 Requirements

| Requirement | Details |
|-------------|---------|
| **OS** | Windows 10/11, Server |
| **Privileges** | Administrator |

---

## 🚀 Usage

```cmd
:: Run as Administrator
Consent.cmd
```

---

## 🔧 What It Does

1. Takes ownership of `%windir%\system32\consent.exe`
2. Resets and restricts ACLs (Console Logon only)
3. Sets registry:
   - `ConsentPromptBehaviorAdmin` = 5
   - `ConsentPromptBehaviorUser` = 1

---

<p align="center">
  <sub>🛡️ Gorstak Windows Security Tooling</sub>
</p>

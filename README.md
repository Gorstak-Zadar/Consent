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

---

## Disclaimer

**NO WARRANTY.** THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.

**Limitation of Liability.** IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.

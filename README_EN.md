# 🇬🇧 English version

## 🌟 Description

> **Legit DLC unlocker** for the Steam version of **Hearts of Iron IV** on macOS.  
> Powered by **CreamAPI v5.3.0.0** — no game files are modified, just the Steam library.

This tool unlocks **all DLCs** for your legally purchased Steam copy of Hearts of Iron IV on macOS.  
It replaces the original `libsteam_api.dylib` with a modified **CreamAPI** version, tricking the game into thinking you own every DLC.

> ⚠️ **Note:** The actual DLC content files must already be present in the game folder. This tool only enables access to them.

---

## 🔧 How It Works

1. CreamAPI intercepts Steam API calls
2. The game believes all DLCs are legitimately owned
3. You launch HOI4 and enjoy full DLC access

---

## 🙏 Credits

- **[deadmau5](https://cs.rin.ru/forum/viewtopic.php?f=29&t=70576)** — creator of **CreamAPI**
- **[KyLaEga](https://github.com/KyLaEga/EU4-DLC-Unlocker-macOS/tree/master)** — for providing the base files and macOS setup

---

## 🚀 Installation Instructions

### 1️⃣ Download the files
Clone the repo or manually download:
- `cream_api.ini`
- `libsteam_api.dylib`

### 2️⃣ Rename the original library
Go to your game folder (usually `~/Library/Application Support/Steam/steamapps/common/Hearts of Iron IV/`).  
Find `libsteam_api.dylib` and rename it to:

```Copy
libsteam_api_o.dylib
```
### 3️⃣ Copy the new files
Place the downloaded `cream_api.ini` and `libsteam_api.dylib` into the same folder.

### 4️⃣ Launch the game
Via Steam or directly. If macOS asks for permission, go to **Privacy & Security** and allow the library to run.

> 💡 **Tip:** On first launch, Gatekeeper may show a warning — click "Open Anyway" or allow it in System Settings.

---

## ✅ Requirements

| Component                | Condition                                   |
|-------------------------|---------------------------------------------|
| macOS                   | 10.13 (High Sierra) or newer                |
| Hearts of Iron IV       | Legitimate Steam copy                       |
| DLC content             | Physical DLC files must be present in the game folder |

---

## 💻 Supported Platforms

| Platform             | Architecture      | Status                            |
|----------------------|-------------------|-----------------------------------|
| macOS 10.13+         | Intel (x86_64)    | ✅ Fully supported                |
| macOS 11+            | Apple Silicon (M1/M2/M3/M4) | ✅ Fully supported (via Rosetta 2) |

> On Apple Silicon, the game runs under Rosetta 2 — the unlocker is fully compatible.

---

## ❓ FAQ

**Do I need to disable antivirus or SIP?**  
No, CreamAPI does not require disabling system protection.

**Will I get banned from Steam?**  
The tool doesn't directly interact with your account, but use at your own risk.

**DLCs not unlocking?**  
Make sure the DLC files are in `game/dlc/` or a similar folder.

---

## ⚠️ Known Issue

**Paradox Launcher may show an error or fail to display DLCs — this is normal!**

After installing the unlocker, the Paradox Launcher might:
- fail to show installed DLCs in the list;
- display an error like “We were unable to verify ownership of this DLC.”.

**Don’t panic!** 🎯  
Inside the actual game, **all DLCs work perfectly and are fully accessible**. The launcher simply cannot correctly read the license info from the modified Steam library — this does not affect gameplay. Launch the game directly or through the launcher (ignoring any errors) and enjoy the complete content.

---

## 📄 License

This project is for educational purposes only. All rights to CreamAPI belong to **deadmau5**.  
Hearts of Iron IV is a trademark of **Paradox Interactive**.

---

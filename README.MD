# PS4 11.50 - 13.00 WebKit Exploit By OGH

### **🚀 Host Link: [codeogh.github.io/ogh](https://github.io)**

> **⚠️ CREDITS:** This project is a customized fork based on the original base exploit extraction made by **[RawGame]**. Special thanks to the developers of the `lapse` and `poops` exploit chains.

---

## ✨ Features Added By OGH

- **Brand New UI Design:** Implemented a high-definition PlayStation gaming background and integrated a custom OGH circular logo badge.
- **Real-Time Progress Bar:** Added a functional visual loading bar synchronized with the actual browser's offline deployment cache status.
- **Zero-Click Automation:** The interface automatically detects the firmware and boots the appropriate exploit chain after a brief buffer delay (no controller input required).
- **Streamlined Offline Assets:** two lightweight, static fullscreen indicators (`success.jpg` and `failed.jpg`) featuring clean text indicators.
- **Integrated Donations:** Embedded a native, console-friendly golden donation trigger linked directly to PayPal.Me.

---

## 🛠️ Project Structure



├── index.html          # Automated home layout with progress bar & PayPal
├── run_lapse.html      # Re-designed Lapse chain execution page
├── run_poops.html      # Re-designed Poops chain execution page
├── chain_lapse.js      # Exploit mechanics for 11.50 - 12.02
├── chain_poops.js      # Exploit mechanics for 12.50 - 13.00
├── core.js             # Shared exploit core orchestration
├── mem.js              # Read/Write primitives
├── int64.js            # 64-bit integer helper data types
├── rpc_worker.js       # Background execution pipeline thread
├── ps4_offsets.js      # Firmware configuration registers database
├── payload.bin         # Standard modular target code payload loader
├── patches/            # Hardcoded compilation binary blobs
│   ├── 1100.bin
│   ├── 1150.bin
│   ├── 1200.bin
│   ├── 1250.bin
│   └── 1300.bin
├── cache.appcache      # All-in-one storage manifest for offline hosting
├── logo_raw.png        # Circular yellow & blue OGH brand icon
├── background.jpg      # Immersive PlayStation background wallpaper
├── success.jpg         # Explicit "Jailbreak success" screen graphic
└── failed.jpg          # Explicit "Jailbreak failed" screen graphic
```

---

## 🎮 Supported Firmware Configurations

The framework routes your system user-agent version to the correct target block automatically:

| Firmware | Exploitation Pipeline |
| --- | --- |
| **11.50** | `lapse` chain |
| **11.52** | `lapse` chain |
| **12.00** | `lapse` chain |
| **12.02** | `lapse` chain |
| **12.50** | `poops` chain |
| **12.52** | `poops` chain |
| **13.00** | `poops` chain |

---

## ⚙️ How to use on your PS4

1. Launch your console's native **Web Browser** application.
2. Press the **Options** button on your controller, open settings, and execute both **Delete Cookies** and **Clear Website Data** to prevent old conflicts.
3. Saisissez l'adresse : **https://codeogh.github.io/ogh**
4. Let the loading bar cache files up to `100%`. Once done, you can safely disconnect your PlayStation from the network; your host will load completely offline out of local browser storage memory.

---

## 💛 Support the Developer

If you find this clean, fast, and stylized deployment framework helpful, consider supporting the customization and hosting maintenance efforts:

👉 **[Faire un don avec PayPal](https://paypal.me)**

---

> **Disclaimer:** This project is intended exclusively for research, educational, and legitimate homebrew development purposes. Use it only on hardware and software you own or are explicitly authorized to modify. The authors and distributors assume zero liability for software instabilities, data corruption, or collateral system issues resulting from its usage.

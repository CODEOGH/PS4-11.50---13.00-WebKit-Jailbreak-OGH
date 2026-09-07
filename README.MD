
# PS4 11.50 - 13.00 WebKit Jailbreak OGH

### **You can run this project on your PS4 from our custom host link via GitHub Pages**

> **⚠️ THIS PROJECT WAS ORIGINAL BASE CODE MADE BY [RawGame](https://www.facebook.com/RawGameStore/)**

> **⚠️ CUSTOM PRESENTATION & VISUAL ANIMATIONS DESIGNED BY OGH**

> This is a customized fork that adds an automatic progression bar, zero-click automation, and incorporates the custom OGH branding structure alongside the community exploit assets. Please support the original lapse and poops chain developers.

A browser-based PS4 jailbreak project targeting firmware versions in the **11.50–13.00** range, customized with a fully automated UI, custom OGH branding logo, and an integrated real-time cache progress indicator.

The project combines firmware-specific offsets, JavaScript exploitation chains, memory primitives, and kernel payloads into a self-contained web-based loader. It is designed to run directly from the native PS4 web browser and includes completely offline caching so the required assets can remain available after the initial load even without an internet connection.

> **Disclaimer:** This project is intended for research, educational, and legitimate homebrew development purposes. Use it only on hardware and software you own or are authorized to modify. The authors and distributors are not responsible for damage, data loss, or other consequences resulting from its use.

## Features

- **Automated Execution:** Zero interaction required. The exploit launches itself after a 3-second buffer.
- **Visual Progress Bar:** Real-time feedback showing caching percentage directly on your screen.
- **Custom OGH Branding:** Replaced placeholders with custom high-definition brand assets.
- Support for both `lapse` and `poops` memory corruption chains.
- Firmware-specific WebKit and kernel offsets up to 13.00.
- JavaScript memory read/write primitives.
- Worker-based RPC support for memory operations and execution pivots.
- Kernel patch blobs for supported firmware versions built directly into the server files.
- Offline browser caching through the updated Application Cache manifest.

## Troubleshooting

Most issues on the PlayStation 4 web browser are usually solved by pressing the **Options** button on your controller, going into settings, and selecting **Delete Cookies** and **Clear Website Data**. If you encounter repeated "Not Enough System Memory" errors, simply restart your console and reload your custom link.

## Supported Firmware

The launcher currently routes firmware versions automatically as follows:

| Firmware | Chain |
| --- | --- |
| 11.50 | `lapse` |
| 11.52 | `lapse` |
| 12.00 | `lapse` |
| 12.02 | `lapse` |
| 12.50 | `poops` |
| 12.52 | `poops` |
| 13.00 | `poops` |

*Note: Firmware 11.00 offsets are present inside the file structure and could theoretically be triggered.*

## Project Structure

```text
.
├── index.html
├── run_lapse.html
├── run_poops.html
├── chain_lapse.js
├── chain_poops.js
├── core.js
├── mem.js
├── int64.js
├── rpc_worker.js
├── ps4_offsets.js
├── payload.bin
├── patches/
│   ├── 1100.bin
│   ├── 1150.bin
│   ├── 1200.bin
│   ├── 1250.bin
│   └── 1300.bin
├── cache.appcache
├── logo_raw.png
└── EXTRACTION_MANIFEST.json
```


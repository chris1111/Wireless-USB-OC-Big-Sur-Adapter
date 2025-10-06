## USB mode switching for Wi‑Fi adapters

Some USB Wi‑Fi adapters initially enumerate as a virtual CD‑ROM or USB flash drive containing proprietary Windows drivers. To make the adapter appear as a usable network device you must send it a mode‑switch signal. In many cases a simple USB "eject" (removing the virtual storage) is enough; some devices require a vendor‑specific command.

For an easy eject-based solution on macOS, try [Eject2Net](https://github.com/MyLittleCrab/Eject2Net) — lightweight and simple to use.

For adapters that need non-standard or vendor-specific signals, see [usb_modeswitch](https://github.com/MyLittleCrab/usb_modeswitch_macos) — more powerful but more complex to learn.

Quick checklist:

- If your adapter shows up as a CD/USB drive, try an eject-based tool first.
- If eject doesn't work, use usb_modeswitch_macos and follow the device-specific instructions.

# Pwnagotchi Lab (Pi Zero 2 W) — USB RNDIS + Headless Provisioning
**Building in public**: documenting a reproducible headless build using a Raspberry Pi Zero 2 W and Pwnagotchi for authorized security learning.

This repository focuses on:
- USB Ethernet (RNDIS) headless provisioning
- Secure SSH onboarding on modern images
- systemd service validation and logs
- Safe research framing and defensive learning outcomes

> ⚠️ Ethics & scope: This project is for **authorized testing only** (networks you own or have explicit permission to assess). The documentation here focuses on **setup, reliability, and defensive understanding**, not misuse.

---

## Hardware
- Raspberry Pi Zero 2 W
- microSD (16–128GB)
- USB data cable (OTG capable)
- Windows host (RNDIS driver)

---

## Software
- Pwnagotchi (version documented in `/docs/validation.md`)
- OpenSSH
- systemd
- USB gadget mode: `dwc2` + `g_ether`

---

## Network Architecture (USB-only)
## Windows Host (RNDIS)
- IP: 10.0.0.1
- | USB

- Pi Zero 2 W (usb0)
- IP: 10.0.0.2



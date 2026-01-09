# VALIDATION CHECKLIST

## Windows host
- [ ✅] Device Manager shows **USB Ethernet / RNDIS Gadget**
- [ ✅] Adapter status is **Up**
- [ ✅] Host IP on RNDIS is `10.0.0.1`

PowerShell:
```powershell
ipconfig
arp -a
ping 10.0.0.2
ssh pi@10.0.0.2

Device

After SSH login:
	•	Confirm identity/banner (version)
	•	Confirm systemd management (service exists)
	•	Confirm logs can be accessed

Example commands:
uname -a
hostname
systemctl status pwnagotchi



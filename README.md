# Mitel 6800 & 6900 Series SIP Firmware Archive (v4.x)

This repository contains archived **4.x SIP firmware** for Mitel 6800 and 6900 Series IP phones.

Due to GitHub file size limitations, the firmware archive has been split into separate repositories by major version:

- 🔹 v4 Firmware: https://github.com/el3ctrofuzz/mitel-sip-v4-firmware-archive
- 🔹 v5 Firmware: https://github.com/el3ctrofuzz/mitel-sip-v5-firmware-archive
- 🔹 v6 Firmware: https://github.com/el3ctrofuzz/mitel-sip-v6-firmware-archive

Many of these firmware versions are no longer publicly available or are extremely difficult to source through official channels. This archive preserves legacy builds required for device recovery, firmware stepping, and compatibility upgrades.

Please drop a star if you found this useful.

---

## Supported Mitel SIP Phone Models

### Mitel 6800 Series
- 6863i
- 6865i
- 6867i
- 6869i
- 6873i

### Mitel 6900 Series
- 6905
- 6910
- 6915
- 6920
- 6920w
- 6930
- 6930w
- 6940
- 6940w
- 6970

---

## Firmware Versions Included (4.x Series)

- 4.2.0.2023-SIP
- 4.3.0.1063-SIP
- 4.3.0.1071-SIP
- 4.3.1075
- 4.3.1077

Firmware files are provided in original `.st` format per model.

---

# Critical Firmware Upgrade Path (Recovery & Stepping)

After hardware reset, devices revert to firmware version 4.3.

You MUST follow this exact upgrade sequence:

1. **Hardware Reset → Firmware 4.3**
2. Upgrade to **5.1.0** (specifically 5.1.0 — NOT 5.0 or other 5.x builds)
3. Upgrade to **6.1.x** (6867i successfully upgraded from 5.1.0 to 6.5.0.5013 from hardware reset)

---

# Security Warning

Do NOT remain on firmware 4.x in production environments.

Multiple vulnerabilities exist in older firmware, including:

- CVE-2024-37569 (affecting Mitel 6869i firmware)

Example reference:
https://www.cvedetails.com/cve/CVE-2024-37569/

Always upgrade to the latest 6.4.x release where possible.

---

# Intended Use

This repository exists for:

- Firmware recovery
- Legacy device restoration
- Stepping-stone upgrades
- Preservation of deprecated builds
- Lab and research use

This is not affiliated with or endorsed by Mitel.

---

# Disclaimer

Firmware remains the property of Mitel Networks Corporation.

This archive is provided for preservation and interoperability purposes.  
Use at your own risk.

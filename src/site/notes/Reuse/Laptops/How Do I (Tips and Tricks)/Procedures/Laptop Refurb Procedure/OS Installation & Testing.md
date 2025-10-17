---
{"dg-publish":true,"permalink":"/reuse/laptops/how-do-i-tips-and-tricks/procedures/laptop-refurb-procedure/os-installation-and-testing/","tags":["procedure","software","testing"]}
---


# OS Installation & Testing

Install operating system and complete hardware testing with QA Helper.

## 🚀 Boot to Installation Environment

### Setup Connections
- [ ] **Power cable** connected
- [ ] **USB installation media/drive** (USB-C or USB-A)
- [ ] **Ethernet cable** (internet required)

### Boot Process
1. Power on laptop
2. Repeatedly press **Boot Menu key** (F12 for Dell/Lenovo, F9 for HP)
3. Select **UEFI USB boot device** (may show as "USB Drive" or "Realtek")
4. Choose **Linux Mint** (default) or **Windows** (if specifically instructed)

## 🛠️ QA Helper Testing

### Installation Options
- **Test in live environment** first, then install OS
- **Install OS immediately**, then test in full system
- **Note:** Some tests require full OS installation (video ports, certain drivers)

### Quick Test Sequence
1. [ ] **Check drive health** in QA Helper
   - **Orange text** = unhealthy drive → replace and notify IT
2. [ ] **Click "Install OS"** - target the SSD
3. [ ] **Wait ~15 minutes** for installation

### Comprehensive Testing
After OS installation, complete all QA Helper tests:

- [ ] **CPU stress test** (5 minutes - test ports during this time)
- [ ] **Speaker testing**
- [ ] **Camera verification**
- [ ] **USB port functionality**
- [ ] **Video output ports** (HDMI, DisplayPort)
- [ ] **Network connectivity**
- [ ] **Battery health check**

## 🔧 Troubleshooting Tips

- **Sound issues**: May need manufacturer drivers from official website
- **Driver problems**: Some hardware only works with full OS installed
- **Multiple drives detected**: May indicate hidden drive → **STOP and report to SDA**

## ❌ Failed Testing?
- **Minor issues**: Note on spec sheet and continue
- **Major issues**: Laptop → **Recycle Bin**

## ✅ All Tests Passed?
Proceed to **[[Reuse/Laptops/How Do I (Tips and Tricks)/Procedures/Laptop Refurb Procedure/Inventory & Final Steps\|Inventory & Final Steps]]**

> [!tip]- RAM Consideration
> If installing Linux AND laptop has ≥8GB RAM, you can remove USB drive once QA Helper loads. For Windows or <8GB RAM, keep USB connected until installation completes.
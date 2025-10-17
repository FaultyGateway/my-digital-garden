---
{"dg-publish":true,"permalink":"/reuse/laptops/how-do-i-tips-and-tricks/procedures/laptop-refurb-procedure/bios-uefi-configuration/","tags":["procedure","bios","uefi","configuration"]}
---


# BIOS/UEFI Configuration

Essential firmware settings for laptop boot preparation.

## ⌨️ BIOS Access Keys

| Brand | BIOS Key | Boot Menu Key |
|-------|----------|---------------|
| Dell | F2 | F12 |
| Lenovo | F1 or F2 | F12 |
| HP | F10 | F9 |
| ASUS | F2 or DEL | Varies |
| Other | Try F1/F2 first | Try F12/F9 |
>[!tip] If these aren't working, check the full chart here: [[Reuse/Laptops/How Do I (Tips and Tricks)/Tips/BIOS Key Chart\|BIOS Key Chart]]

## ⚙️ Required Settings

### 1. Security & Access
- [ ] **Clear admin/BIOS passwords** if present
- [ ] Try common passwords: "password", organization defaults
- [ ] Use [bios-pw.org](https://bios-pw.org/) for Dell models if needed

### 2. Boot Configuration
- [ ] Set boot mode to **"UEFI Only"** (CSM Off)
- [ ] If UEFI unavailable: **"Legacy BIOS Only"**
- [ ] Set boot order: **Optical → Hard Drive → USB**
- [ ] **Enable USB Boot Support**

### 3. Hardware Settings
- [ ] **Disable Secure Boot**
- [ ] Set SATA operation to **AHCI**
- [ ] **Disable anti-theft tracking** (Computrace/Absolute)
- [ ] **Disable management features**: MEBx, AMT, Intel ME

### 4. System Checks
- [ ] Verify **date/time** accuracy
- [ ] **Reset to default settings** first
- [ ] **Reboot and re-enter** BIOS to confirm changes

## 🔓 BIOS Password Bypass

If locked out of BIOS settings:
1. Use **Boot Menu key** (F12/F9) to access USB directly
2. Try switching between **UEFI/Legacy modes**
3. **Note the restriction** in system documentation

## ✅ Configuration Complete?
Proceed to **[[Reuse/Laptops/How Do I (Tips and Tricks)/Procedures/Laptop Refurb Procedure/Drive Installation\|Drive Installation]]**

> [!important]- April 2025 Update
> Only change the specified settings above. Ignore any previous configuration guides that include extra steps.
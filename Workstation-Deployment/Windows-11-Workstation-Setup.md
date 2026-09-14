# Windows 11 Workstation Deployment

## Overview

Reimaged and prepared a previously assigned Dell OptiPlex workstation for organizational use.

The work included a clean Windows 11 installation, storage troubleshooting, network connectivity, and initial Windows configuration.

---

## Environment

- Dell OptiPlex workstation
- Windows 11 Pro
- 512 GB Micron NVMe SSD
- UEFI
- Bootable Windows 11 USB
- Wired Ethernet connection

---

## Work Completed

### Windows 11 Deployment

Verified the existing operating system before starting the reimage.

Connected the Windows 11 installation media and accessed the Dell One-Time Boot Menu using `F12`.

Booted from the USB in UEFI mode and started a clean Windows 11 installation.

---

### Storage Troubleshooting

During Windows Setup, the internal 512 GB SSD was not available as an installation destination.

Only the 28.9 GB Windows installation USB was displayed.

I stopped the installation at this point to avoid making changes to the wrong drive.

Verified that the 512 GB Micron SSD was detected by the Dell pre-boot environment.

Accessed the BIOS and reviewed the SATA/NVMe storage configuration.

The system was configured with RAID enabled.

Tested AHCI/NVMe configuration as part of the troubleshooting process.

When this did not resolve the issue, the approved/default storage configuration was restored.

After rebooting and returning to Windows Setup, the internal SSD was successfully detected.

---

### Windows Installation

Selected the approved partition on the internal SSD.

Completed the Windows 11 installation and allowed the workstation to complete the required restart process.

---

### Network Configuration

During Windows Out-of-Box Experience (OOBE), the workstation initially had no network connection.

Connected the workstation directly to the wired office network using Ethernet.

Verified that the network connection was established and continued the Windows setup.

---

### Organizational Setup

Continued through Windows Out-of-Box Experience.

Selected **Set up for work or school** to prepare the workstation for organizational use.

The workstation was then ready for the next stage of company configuration.

---

## Issue and Resolution

### Issue

The internal 512 GB NVMe SSD was not visible during Windows 11 installation.

### Investigation

- Confirmed the Windows installation USB was detected.
- Confirmed the internal SSD was detected at the firmware level.
- Reviewed the BIOS storage configuration.
- Checked RAID and AHCI/NVMe configuration.
- Rebooted and verified storage detection in Windows Setup.

### Resolution

After restoring the required storage configuration and rebooting the workstation, Windows Setup detected the internal SSD.

The Windows 11 deployment was then completed successfully.

---

## Technologies Used

`Windows 11 Pro` • `Dell OptiPlex` • `UEFI` • `Dell BIOS`

`Windows Installation Media` • `NVMe SSD` • `RAID/AHCI`

`Ethernet` • `Windows OOBE`

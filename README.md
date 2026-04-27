# 🖥️ OSSP Comprehensive Project: Bodhi Linux Virtualization & Deployment
**Author:** Yeabisira Challachew  
**Focus:** Operating Systems, Virtualization, and System Configuration

---

## 📖 Executive Summary
This project explores the practical application of **Operating System and System Programming (OSSP)** concepts by deploying **Bodhi Linux 7.0.0** within a virtualized environment. The core objective was to successfully configure a Hypervisor (VirtualBox), allocate hardware resources, and execute a full OS installation while documenting system behavior and troubleshooting performance bottlenecks.

---

## 🎯 Project Objectives
1. **Hypervisor Setup:** Installing and configuring Oracle VM VirtualBox as the base layer.
2. **Environment Virtualization:** Creating a Virtual Machine (VM) with optimized resource settings.
3. **OS Deployment:** Executing a clean install of Bodhi Linux using the `ext4` filesystem.
4. **Problem Solving:** Identifying and resolving graphical performance issues through hardware acceleration settings.

---

## 🛠️ Detailed Technical Workflow

### Phase 1: Environment Preparation
* **Source Acquisition:** Downloaded the Bodhi Linux ISO (Standard Release) and VirtualBox binaries.
* **Hypervisor Installation:** Set up the VirtualBox environment on the host machine, ensuring all network interfaces and dependencies were correctly configured.

### Phase 2: Virtual Machine Architecture
In this stage, specific hardware parameters were defined to ensure the guest OS runs efficiently:
* **Memory (RAM):** Allocated 2.0 GB to balance host and guest performance.
* **Processor:** 1 Virtual CPU core assigned.
* **Storage:** Created a 20 GB Virtual Disk Image (VDI) with dynamic allocation.
* **Video Tuning:** Initially set to default, later manually adjusted to **128 MB** to support the Enlightenment Desktop Environment (Moksha).

### Phase 3: Linux Installation Process
* **Booting:** Initialized the VM using the ISO file.
* **Partitioning:** Formatted the virtual drive using the `ext4` journaling filesystem.
* **Localization:** Configured timezone (Addis Ababa) and keyboard layouts.
* **User Identity:** Established a root-level user account under the name **Yeabisira Challachew**.

---

## 📂 Documentation Structure
* 📊 **Resource_Allocation.xlsx**: A technical spreadsheet detailing every hardware parameter assigned to the VM.
* 📑 **Bodhi_Installation_Report.pdf**: A comprehensive, step-by-step visual guide containing all screenshots of the installation phases.

---

## 🔧 Troubleshooting Spotlight: "The Video Memory Fix"
> **Issue:** During the first boot attempt, the UI was lagging, and window rendering was slow.  
> **Diagnosis:** The default Video Memory (16MB) was insufficient for the Moksha Desktop's compositing effects.  
> **Resolution:** Accessed the VM Settings > Display and increased the **Video Memory to 128MB**. This stabilized the frame rate and provided a smooth user experience.

---

## 🏆 Conclusion
The project was completed successfully. The Bodhi Linux environment is now fully functional, providing a lightweight yet powerful Linux distribution for further system programming tasks. 

---
*Submitted as part of the OSSP Course Requirement.*

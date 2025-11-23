## Labbing Instructions: 4.2 Understanding Computer Hardware (weight: 2)

---

>💬 **Tip:** Paste this study guide into ChatGPT and ask for **more instructions** by specifying:  
>- “Provide step-by-step lab instructions for this objective.”  
>- “Include which Linux distro to use (Debian/Ubuntu or RHEL/Fedora).”  
>- “Show examples of installing, verifying, and managing desktop and server applications.”  
>- “Include minimal command-line practice for package management and development tools.”  
>- “Focus only on what is most important for passing the LPI Linux Essentials exam.”  

>This will prompt ChatGPT to give **practical, exam-focused lab steps** for each section.

---

**Objective:** Explore and identify computer hardware components in Linux.

**Step-by-Step Lab Instructions:**

1. 🧠 **Check CPU information**  
   - Command: `lscpu`  
   - Observe: CPU model, cores, architecture, cache size.

2. 💾 **View memory (RAM) details**  
   - Command: `cat /proc/meminfo`  
   - Observe: Total memory, free memory, available memory.

3. 💽 **List storage devices and partitions**  
   - Command: `lsblk`  
   - Observe: Disk names (`/dev/sda`, `/dev/sdb`), partitions, mount points.

4. 🖥️ **Check PCI devices (graphics, network, peripherals)**  
   - Command: `lspci`  
   - Observe: Device type, vendor, model.

5. 🛠️ **Verify loaded drivers**  
   - Command: `lsmod`  
   - Observe: Kernel modules managing hardware.

6. 🖱️ **Test peripheral detection**  
   - Plug in a USB device.  
   - Command: `dmesg | tail`  
   - Observe: Kernel messages showing device recognition.

7. 📂 **Check mounted filesystems and storage usage**  
   - Command: `df -h`  
   - Observe: Partition size, usage, mount points.

8. ⚡ **Optional: Identify power supply and motherboard info**  
   - Command: `sudo dmidecode -t system` (requires root)  
   - Observe: Manufacturer, model, BIOS version, serial number.

**Tips:**  
- Use `man` for command options (`man lscpu`, `man lsblk`).  
- Compare outputs between virtual machine and physical hardware if possible.  
- Focus on identifying hardware names, types, and connection points — this is exam-relevant.

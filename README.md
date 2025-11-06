# OS Commands Cheat Sheet

---

## **1. ps – Process Status**
- `ps` → Show processes in the current terminal.  
- `ps -e` → Show all system processes.  
- `ps -f` → Full-format listing with more details.  
- `ps -ef` → All processes in full format.  
- `ps -aux` → Detailed view with CPU and memory usage.  
- `ps id` → Show processes with a specific PID.  
- `pidof <process>` → Get PID of a running process.  
- `ps -H` → Show processes in hierarchical/tree format.  
- `ps -T` → Show threads of the current terminal.

---

## **2. top – Real-Time Process Monitoring**
- `top` → Start real-time process monitoring.  
- Press `P` → Sort processes by CPU usage.  
- Press `M` → Sort processes by memory usage.  
- Press `k` → Kill a process directly from top.

---

## **3. df – Disk Free Space**
- `df` → Show disk usage of mounted file systems.  
- `df -h` → Human-readable format (KB/MB/GB).  
- `df -hT` → Show usage with file system type.  
- `df -i` → Show inode usage.  
- `df -h --total` → Show total disk usage.  
- `df -ah` → Show all disk usage including pseudo file systems.

---

## **4. uname – System Information**
- `uname -a` → Show all system info.  
- `uname -r` → Kernel version.  
- `uname -s` → OS name.  
- `uname -n` → Hostname.  
- `uname -v` → Kernel version string.  
- `uname -p` → Processor type.  
- `uname -o` → Operating system.

---

## **5. free – Memory Usage**
- `free` → Show total, used, and free memory.  
- `free -s 5` → Repeat memory stats every 5 seconds.  
- `free -g` → Show memory in GB.  
- `free -m` → Show memory in MB.  
- `free -k` → Show memory in KB.

---

## **6. lspci – PCI Devices**
- `lspci -v` → Verbose PCI device info.  
- `lspci -vv` → Very verbose PCI details.  
- `lspci -nn` → Show PCI numeric IDs.  
- `lspci -k` → Show kernel driver used by devices.

---

## **7. kill – Terminate Processes**
- `kill <PID>` → Gracefully terminate a process.  
- `kill -9 <PID>` → Force kill a process immediately.  
- `kill -l` → List all signals.  
- `killall firefox` → Kill all processes named "firefox".

---

**Tip:** Combine commands for monitoring and troubleshooting:
- Example: `ps -ef | grep firefox` → Find Firefox process PID.  
- Example: `df -h` → Quickly check free disk space before installing software.  
- Example: `top` → Keep an eye on CPU/memory usage in real-time.

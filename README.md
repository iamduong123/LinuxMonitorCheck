# Linux System Monitor

**A DevOps‑style Bash script to monitor CPU, memory, and disk usage with alerting and logging.**

## 🚀 Project Overview

This script continuously monitors resource usage on a Linux system, alerts when usage exceeds thresholds, and logs usage to a file. It’s designed to simulate real-world DevOps monitoring processes and improve system observability.

## 📋 My Role & Learning

- Built the entire script myself in Bash.  
- Learned how to reliably parse system metrics (CPU, memory, disk) using standard Linux tools.  
- Implemented logging with timestamps and optionally log rotation.  
- Designed threshold-based alerting to notify on high usage.  
- Gained deeper understanding of system resource behavior under load.

## 🛠︎ Technical Details

- **Language**: Bash  
- **Tools**: `top`, `free`, `df`, `awk`  
- **Logging**: Writes to a configurable log file  
- **Thresholds**: CPU, memory, disk thresholds are configurable at the top of the script  
- **Loop**: Runs indefinitely with a sleep interval (configurable)

## 💻 How to Run

1. Clone the repo  
   ```bash
   git clone https://github.com/your-username/linux-system-monitor.git
   cd linux-system-monitor

# Linux System Monitor 🖥️

**A Bash-based monitoring tool for CPU, memory, and disk usage** — provides real-time alerts and logs usage metrics to a file. Designed as a DevOps-style portfolio project to demonstrate automation, scripting, and system observability.

---

## Table of Contents

1. [Overview](#overview)  
2. [Motivation & What I Learned](#motivation--what-i-learned)  
3. [Features](#features)  
4. [Technical Details](#technical-details)  
5. [Usage](#usage)  
   - [Prerequisites](#prerequisites)  
   - [Running the Script](#running-the-script)  
   - [Configuration](#configuration)  
   - [Managing Logs](#managing-logs)  
6. [Example Log Output](#example-log-output)  
7. [Future Improvements](#future-improvements)  
8. [Reflection](#reflection)  
9. [Contributing](#contributing)  
10. [License](#license)  
11. [Contact](#contact)  

---

## Overview

This project is a lightweight, continuously running Bash script that monitors key system resources on a Linux machine:

- **CPU usage**  
- **Memory usage**  
- **Disk usage**

If usage crosses predefined thresholds, the script issues a terminal alert. Meanwhile, every monitoring cycle is logged to a timestamped file, making it easy to review historical system behavior.

This repository demonstrates important DevOps competencies: automation, monitoring, alerting, and logging.

---

## Motivation & What I Learned

I built this tool as my *first DevOps‑style project* to:

- Gain hands-on experience with Linux resource monitoring  
- Learn how to build simple but effective alerting logic  
- Practice writing maintainable Bash scripts  
- Understand how to persist metrics via logging  

Through this project, I became more comfortable parsing system information (`top`, `free`, `df`), managing loops, and writing scripts that behave like a lightweight production agent.

---

## Features

- Periodic monitoring of CPU, memory, and disk  
- Colorized alert messages when thresholds are exceeded  
- Logging with timestamp, for each cycle  
- Configurable thresholds and log path  
- Automatically creates the log file if it doesn’t exist  

---

## Technical Details

- **Language**: Bash  
- **Tools**:  
  - `top` — for CPU metrics  
  - `free` — for memory statistics  
  - `df` — for disk usage  
  - `awk` — for parsing  
  - `date` — for timestamping logs  
- **Loop**: Infinite `while` loop with configurable sleep interval  
- **Logging**: Appends usage data with timestamps  
- **Alerting**: Prints to console using colored output (`tput`) when thresholds are exceeded  

---

## Usage

### Prerequisites

- Any Linux system  
- Bash shell  
- Basic utilities: `top`, `free`, `df`, `awk`, `date` (these are usually pre-installed)

---

### Running the Script

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/linux-system-monitor.git
   cd linux-system-monitor
2. Run the script:
   ```bash
   ./system_monitor.sh

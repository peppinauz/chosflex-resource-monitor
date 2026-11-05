# ChromeOS Flex & Crostini System Resource Monitor

Monitor system resources (CPU, Memory, Disk, Network Traffic) and running Docker containers from a beautiful, responsive web interface tailored for ChromeOS Flex (MacBook Air 2018 / Crostini Debian VM).

## Features

- **Real-Time System Metrics**: CPU utilization, load average, core count, RAM usage, storage allocations (Host vs Crostini LXC), and network throughput (`/proc/net/dev`).
- **Active Processes**: Top system processes running inside Crostini with CPU% and Memory%.
- **Docker Containers**: Dedicated section monitoring running Docker containers (ID, Name, Image, Status, Ports).
- **Auto-Refresh**: Automatically updates every 5 seconds (configurable from 0.5s to 5.0s).
- **Accessible from ChromeOS Flex**: Run the lightweight Python server and open http://localhost:8050 in your ChromeOS browser.

## Quick Start

1. Open your Crostini (Debian) terminal in ChromeOS Flex.
2. Start the Python monitoring server:
   ```bash
   python3 server.py
   ```
3. Open your browser in ChromeOS Flex and go to:
   ```
   http://localhost:8050
   ```

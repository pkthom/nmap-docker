# Docker Nmap Scanner

A simple Docker Compose setup for full-port scanning and service detection.

## Quick Start

1. Create a results directory:
```Bash
mkdir results
```

2. Run the scan:

Specify your target IP or domain using the TARGET environment variable.
```Bash
TARGET="1.2.3.4" docker compose up
```

3. Check results:

```Bash
cat results/scan_res.txt
```

## Configuration

- Full Scan: Scans all 65,535 ports by default (-p-).
- Version Detection: Detects service versions (-sV).
- Performance: Set to aggressive timing (-T4) for faster results.

## Security Warning
[!CAUTION]
Authorized use only. Do not scan targets you do not own or have explicit permission to audit.

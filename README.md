# linux-sys-bench

Linux system diagnostics, kernel resource profiler, and asynchronous API integration engine for performance benchmarking.

## Overview
`linux-sys-bench` automates system metric collection, process telemetry inspection, and high-concurrency API performance testing across Linux environments.

## Features
- **Linux Metric Collectors**: Inspects CPU scheduling, memory pressure, I/O bottlenecks, and network sockets via `/proc` and `sysfs`.
- **Async API Benchmarking**: High-throughput asynchronous HTTP client evaluating endpoint responsiveness and error budgets under load.
- **Structured Reporting**: Exports normalized performance benchmarks in JSON and Prometheus exposition formats.

## Quickstart
```bash
git clone https://github.com/01Leviathan10/linux-sys-bench.git
cd linux-sys-bench
pip install -r requirements.txt
python3 -m sysbench --duration 60 --export metrics.json
```
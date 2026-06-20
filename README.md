# Docker vs Podman: Performance and Security Analysis

**Bachelor's Final Project**  
Shahid Madani University of Azerbaijan

---

## 📋 Project Overview

This project compares **Docker** and **Podman** in terms of performance and security. The goal was to understand the practical differences between these two container technologies in real-world scenarios.

### 🎯 Main Objectives
- Compare CPU and Memory usage
- Evaluate network performance
- Measure container startup time
- Analyze security features and attack surface

---

## 🛠️ Technologies Used
- **Docker** 24.0.5
- **Podman** 4.2.0
- Ubuntu 22.04 LTS
- Benchmarking tools: sysbench, stress-ng, iperf3, htop

---

## 📊 Key Results


- **CPU Performance**: Docker slightly better in some tests
- **Memory Usage**: Podman generally lighter
- **Security**: Podman has advantages (rootless by default)

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/MahdiAmini12/docker-vs-podman-security-performance.git

cd docker-vs-podman-security-performance

# Make scripts executable
chmod +x 1-src/*.sh

# Run benchmarks
./1-src/run_benchmarks.sh

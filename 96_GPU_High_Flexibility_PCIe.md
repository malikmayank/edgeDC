
# 96-GPU Edge Datacenter in a 20-ft Container (Option B: PCIe GPU Servers)

## 🧠 Compute Configuration

- **12x 4U GPU Servers**
  - Each with 8x NVIDIA H100 PCIe GPUs (96 GPUs total)
  - 2x AMD EPYC CPUs per server
  - 1 TB RAM per server

## 🗄️ Rack Configuration

- 3x 42U Server Racks
  - Shock-mounted
  - Airflow optimized for hot aisle containment

## 💾 Storage

- 1x NVMe SSD Storage Array
  - 1PB usable capacity, all-flash

## 🌐 Networking

- 3x 100G Leaf Switches (NVIDIA Spectrum SN3700)
- 2x 400G Spine Switches (NVIDIA Spectrum SN4600)
- 1x OOB Management Switch (1G/10G)

## ❄️ Cooling

- 3x Rear-Door Heat Exchangers
- 1x External Chiller (180kW capacity)

## ⚡ Power Configuration

- 6x High-Density 3-phase PDUs
- 1x 120kVA UPS (15-minute runtime)
- 1x 180kW Diesel Generator with ATS

## 📦 Monitoring & Safety

- Fire Suppression: Novec 1230 Clean Agent System
- Sensors: Temp, Humidity, Smoke, Airflow
- Remote Mgmt: IPMI, VPN, Environmental Monitoring

## 📊 Energy Efficiency & PUE Estimate

| Component                            | Power (kW) |
|--------------------------------------|------------|
| IT Load (GPU, Servers)               | 144        |
| Cooling (Liquid + Fans)              | 30         |
| Power Conversion (UPS, PDU Losses)   | 6          |
| Lighting and Misc                    | 3          |
| **Total Facility Load**              | **183**    |
| **PUE**                              | **1.27**   |

## 📐 Layout

- Cold aisle between racks
- Front-to-back airflow
- Rear access to networking and cooling
- Additional rack space used for PDUs and network aggregation

## 📋 Bill of Materials (Excerpt)

| Qty | Description                         | Part Number        | Vendor     |
|-----|-------------------------------------|--------------------|------------|
| 12  | 4U GPU Server, 8x H100 PCIe GPUs    | SYS-424GP-TNRT     | Supermicro |
| 96  | NVIDIA H100 PCIe GPUs               | H100-PCIe          | NVIDIA     |
| 3   | 42U Server Rack                     | SRV42UBD           | Tripp-Lite |
| 1   | Petabyte NVMe Storage Array         | SSG-121E-NES24R    | Supermicro |
| 3   | Spectrum SN3700 100G Switch         | MSN3700-PB         | NVIDIA     |
| 1   | Vertiv 120kVA UPS + Battery Cab.    | EXL S1-100K-480V   | Vertiv     |
| 3   | Stulz Rear Door Heat Exchanger      | DKM 70             | Stulz      |


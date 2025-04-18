
# 96-GPU Edge Datacenter in a 20-ft Container (NVIDIA-Based)

## 🧠 Compute Configuration (Option A: NVIDIA HGX H100)

- **3x NVIDIA HGX H100 Servers**
  - Each with 8x H100 SXM GPUs (96 GPUs total)
  - 2x Intel Xeon CPUs per node
  - 2 TB RAM per node

## 🗄️ Rack Configuration

- 2x 42U Server Racks
  - Shock-mounted
  - Airflow optimized for hot aisle containment

## 💾 Storage

- 1x NVMe SSD Storage Array
  - 1PB usable capacity, all-flash

## 🌐 Networking

- 2x 100G Leaf Switches (NVIDIA Spectrum SN3700)
- 2x 400G Spine Switches (NVIDIA Spectrum SN4600)
- 1x OOB Management Switch (1G/10G)

## ❄️ Cooling

- 2x Rear-Door Heat Exchangers
- 1x External Chiller (150kW capacity)

## ⚡ Power Configuration

- 4x High-Density 3-phase PDUs
- 1x 100kVA UPS (15-minute runtime)
- 1x 150kW Diesel Generator with ATS

## 📦 Monitoring & Safety

- Fire Suppression: Novec 1230 Clean Agent System
- Sensors: Temp, Humidity, Smoke, Airflow
- Remote Mgmt: IPMI, VPN, Environmental Monitoring

## 📊 Energy Efficiency & PUE Estimate

| Component                            | Power (kW) |
|--------------------------------------|------------|
| IT Load (GPU, Servers)               | 120        |
| Cooling (Liquid + Fans)              | 25         |
| Power Conversion (UPS, PDU Losses)   | 5          |
| Lighting and Misc                    | 2          |
| **Total Facility Load**              | **152**    |
| **PUE**                              | **1.27**   |

## 📐 Layout

- Cold aisle between racks
- Front-to-back airflow
- Rear access to networking and cooling
- LED strip lighting along ceiling

## 📋 Bill of Materials (Excerpt)

| Qty | Description                         | Part Number        | Vendor     |
|-----|-------------------------------------|--------------------|------------|
| 3   | NVIDIA HGX H100 8-GPU Server        | HGX100V8           | NVIDIA     |
| 8   | NVIDIA NVLink Switch                | 900-21530-0020-000 | NVIDIA     |
| 2   | 42U Server Rack                     | SRV42UBD           | Tripp-Lite |
| 1   | Petabyte NVMe Storage Array         | SM-SSG-6429        | Supermicro |
| 2   | Spectrum SN3700 100G Switch         | MSN3700-CS2FC      | NVIDIA     |
| 1   | Vertiv EXL 80kVA UPS + Battery Cab. | EXL080TAS6EI6P     | Vertiv     |
| 1   | Stulz Rear Door Heat Exchanger      | CyberWall          | Stulz      |


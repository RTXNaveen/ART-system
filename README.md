# Automated Rubber Tapping System (ARTS)

## 1. Overview
The Automated Rubber Tapping System (ARTS) is an electromechanical solution engineered to automate the excision of bark on *Hevea brasiliensis* (rubber trees) for controlled latex extraction. The system mounts directly to the trunk, executing programmed incisions at high-yield intervals to maximize output, standardize cutting depth, and reduce manual labor dependencies.

---

## 2. Key Specifications

| Subsystem | Specification |
| :--- | :--- |
| **Form Factor** | Trunk-mounted modular chassis |
| **Primary Power Supply** | Direct Current (DC) Input (12V / 24V bus) |
| **Auxiliary Expansion** | Solar photovoltaic (PV) integration-ready |
| **Cutting Mechanism** | High-precision micro-stepper motor driven blade |
| **Cut Control** | Adjustable depth (0.1 mm increments) and spiral angle |
| **Latex Collection** | Integrated funnel and collection reservoir bracket |
| **Enclosure Rating** | Weatherproof IP65-rated housing |

---

## 3. Power Architecture

### Option 1: Direct Current (DC) Base Configuration
* The base system operates on an external direct current power delivery network.
* Compatible with localized DC bus lines (12V to 24V nominal) or standalone rechargeable DC battery packs.
* Equipped with onboard reverse-polarity protection, over-current regulation, and low-voltage cutoff to safeguard drive motors and control electronics.

### Option 2: Solar Upgrade Pathway
* The power management board includes a dedicated expansion port for solar photovoltaic integration.
* Field upgrades require no structural changes to the chassis; operators can add an external mini solar panel coupled with a compact charge controller and rechargeable Li-ion/LiFePO4 battery pack.
* Enables autonomous off-grid operation suitable for remote plantation grids.

---

## 4. System Architecture

### 4.1 Mechanical Subsystem
* **Mounting Assembly:** Adjustable tension-band clamp accommodating varying tree circumferences without girdling or cambium damage.
* **Actuation Unit:** Two-axis lead screw / belt mechanism providing simultaneous linear downward travel and radial cut progression.
* **Blade Assembly:** Hardened surgical-grade stainless steel blade optimized to excise bark while preserving the inner cambium layer.

### 4.2 Control Subsystem
* **Microcontroller Unit (MCU):** Low-power embedded processor executing real-time task scheduling.
* **Sensors:** Optical limit switches for home positioning; bark surface contact sensors for initial depth calibration.
* **Timer & Scheduling:** Integrated Real-Time Clock (RTC) programmed for nocturnal/pre-dawn actuation cycles (typically 01:00 to 04:00) when turgor pressure produces maximum latex yields.

---

## 5. Operational Workflow

1. **Mounting & Calibration:** Secure the device to the tree trunk above the target tapping panel. Calibrate blade clearance and depth offset.
2. **Scheduling:** Configure cutting frequency and start time via onboard dip switches or digital configuration interface.
3. **Execution:** At scheduled intervals, the MCU commands the blade actuator along the predefined helical cutting track.
4. **Collection:** Latex flows along the newly formed spiral groove into the spouted collection vessel.
5. **Retraction & Sleep:** Blade auto-retracts to home position, and the system enters deep-sleep mode to preserve DC power reserves until the next cycle.

---

## 6. Maintenance & Safety Precautions

* **Blade Inspection:** Inspect blade sharpness every 90 days or after approximately 45 tapping cycles to prevent ragged cuts.
* **Bark Preservation:** Verify depth limiters during installation to ensure incisions do not penetrate beyond the latex vessels into the wood layer.
* **Seal Integrity:** Inspect silicone gaskets periodically to maintain the IP65 environmental rating against plantation humidity and monsoonal rainfall.

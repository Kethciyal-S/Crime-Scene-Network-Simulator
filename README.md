# Crime-Scene-Network-Simulator
Cisco Packet Tracer simulation of a crime scene network featuring VLANs, DNS, and HTTP server configurations.

## 📌 Project Overview
This project is a Cisco Packet Tracer simulation of a Crime Scene Network. It demonstrates network topology design, VLAN segmentation, and server configuration for a secure investigative environment. 

*Note: The full project report with screenshots is available above as a PDF.*

## 🖧 Network Topology
*   **Router:** Cisco 2911
*   **Switch:** Cisco 2960 (Layer 2)
*   **End Devices:**
    *   Investigator-PC
    *   Forensic-PC
    *   Evidence-Server (DNS + HTTP)
    *   Backup-Server
    *   Employee PCs (1-4)
    *   Victim-PC
    *   Suspect-PC

## ⚙️ Configurations
### VLANs
*   **VLAN 10 (Investigation):** Assigned to Investigator, Forensic, and Evidence Server ports.
*   **VLAN 20 (Administration):** Assigned to Employee and Backup Server ports.
*   *Note: All unused ports are assigned to VLAN 999 (Parking Lot) and shut down for security.*

### Server Services (Evidence-Server)
*   **DNS:** 
    *   `backup.local` -> `192.168.20.10`
    *   `evidence.local` -> `192.168.10.10`
    *   `forensic.local` -> `192.168.10.10`
*   **HTTP:** Hosting the evidence database (simulated).

## 📂 Files in this Repository
*   `CrimeSceneNetworkSimulator.pkt` - The main Cisco Packet Tracer file. Download and open this in Packet Tracer.
*   `Project-1 Crime Scene Network Simulator.pdf` - Detailed project report and screenshots.

## 🚀 How to Test
1. Download and install Cisco Packet Tracer.
2. Clone or download this repository.
3. Open `CrimeSceneNetworkSimulator.pkt` in Packet Tracer.
4. Use "Real-time" mode to test connectivity (e.g., ping `evidence.local` from the Investigator PC).

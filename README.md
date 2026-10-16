# Mekanism Reactor Control System (CC:Tweaked)

A highly advanced, modular, and multi-screen control system for **Mekanism Fission Reactors and Industrial Turbines** in Minecraft, powered by **CC:Tweaked** (ComputerCraft). 

Originally developed for the [AKW: Atomic Kinetic Works](https://github.com/MCFabik/AKW-Ultimate-Tech-Design) modpack, this system is designed for massive industrial setups, offering real-time telemetry, automated safety protocols, and a dedicated network architecture.

## 🚀 Features

*   **Interactive Installer:** No more manual code editing! A user-friendly setup menu automatically configures your systems.
*   **Modular Architecture:** Run different dashboards on separate computers/monitors across your facility, all communicating via Wired Modems.
*   **Main RTU (Remote Terminal Unit):** Core logic, burn rate control, redstone SCRAM, and emergency stop integration.
*   **Safety & Radiation Dashboard:** Simulates thermal decay, ECCS (Emergency Core Cooling System), and monitors reactor damage/hall pressure.
*   **MCP & Condenser Dashboard:** Real-time monitoring of your water return loops and drum separators.
*   **Turbine Dashboard:** Tracks energy production, steam flow, and dumping modes across multiple Industrial Turbines.

## 🛠️ Installation

You don't need to manually download these scripts to your Minecraft world. Simply place an **Advanced Computer** connected to your network and run the following command:

```text
pastebin run wx5mnuLj
```

The installer will guide you through the setup process, asking for your facility name, unit number, peripheral IDs, and modem channel. It will automatically download the required files and place them in your `/startup/` folder for auto-reboot functionality.

## 📡 Hardware Requirements & Setup

1.  **CC:Tweaked & Mekanism** are required.
2.  **Networking:** All computers (RTU and Dashboards) must be connected via CC **Wired Modems** and Networking Cables. 
3.  **Monitors:** Use Advanced Monitors (highly recommended) for the dashboards.
4.  **Logic Adapters:** The RTU requires a Fission Reactor Logic Adapter to read the core data.

## ⚙️ Configuration (Post-Install)

If you are running the **Turbine** or **Condenser** dashboards, you will need to specify which Turbine Valves to read from. 
After running the installer, type:
`edit startup/Mekanism-Turbine-Dashboard.lua` (or Condenser)
and update the `TURBINE_VALVES` table with your actual peripheral names.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

# 📂 Smart File Organizer

![Python Version](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Maintained](https://img.shields.io/badge/Maintained%3F-yes-brightgreen.svg?style=for-the-badge)

**Smart File Organizer** is a robust Python automation solution designed for intelligent file categorization. Developed by a Support Analyst focused on efficiency, it handles high-volume directories (like Downloads) by automatically sorting files into specific sub-directories based on extensions, ensuring data integrity and traceability.

## 🚀 Key Features

* **Intelligent Categorization:** Automatic mapping to folders such as `Images`, `Documents`, `Code`, and `Spreadsheets`.
* **Zero Dependencies:** Relies strictly on the Python Standard Library (`os`, `shutil`, `logging`), making it highly portable.
* **Collision Prevention:** Implements an automatic renaming system (e.g., `report_1.pdf`) to prevent data loss.
* **Active Download Protection:** Automatically filters temporary extensions (`.crdownload`, `.part`, `.tmp`) to avoid corrupting files in transfer.
* **Production-Grade Logging:** Uses the `logging` module to generate a clear audit trail of all moved files.
* **Exception Handling:** Built-in logic to handle files currently in use by the system without crashing.

## ⚙️ Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/davi-galvani/file-organizer.git](https://github.com/davi-galvani/file-organizer.git)
   cd file-organizer
Run the script:

Bash
python file_organizer.py
[!IMPORTANT]
The script defaults to the ~/Downloads directory. To target a different folder, update the BASE_DIR variable in the source code.

🛠️ Customization
The script follows the "Open-Closed Principle," making it easy to extend. To add new file types, edit the EXTENSION_MAP dictionary:

Python
EXTENSION_MAP = {
    "Video_Projects": [".prproj", ".aep", ".veg"],
    "Database_Backups": [".sql", ".bak", ".dump"]
}
📈 Roadmap (Future Updates)
As a Database Systems student at Fatec Bauru, I plan to evolve this project with:

Database Logging: Migrating logs from .txt to an SQLite database for advanced statistics.

Real-time Monitoring: Integrating the watchdog library to trigger organization instantly.

CLI Arguments: Support for argparse to define target paths via terminal.

💼 Looking for a Custom Solution? ($24 Basic Setup)
This script is a Basic Version for local use. For clients on Upwork looking for a professional, "set-and-forget" automation, I offer a Premium Implementation Service which includes:

Custom Mapping: Tailored logic for your specific industry (Legal, Design, etc.).

Remote Setup: Complete installation and configuration on your machine.

Execution Scheduling: Setting up a background task (Daemon/Cron) for 100% automation.

Direct Support: 15 days of technical support for any adjustments.

Contact me on Upwork to get started!

Developed by Davi Galvani
Support Analyst @ Ikatec | Database Systems @ Fatec Bauru

# ⚽ OpenLigaDB Automated Football Data
### Built with Make.com → Airtable → Gmail

This project demonstrates a full no-code data automation pipeline using **OpenLigaDB**, **Make.com**, **Airtable**, **Google Sheets** and **Gmail**.

It was created as a portfolio project for a No-Code Developer role.

---

## 🚀 Features

### ✔ 1. Automated Match Importer
The pipeline fetches football match data from:
https://www.openligadb.de/api/getmatchdata/bl1/2025


### ✔ 2. Real-Time Notifications
Whenever a match ends, an email is automatically sent via Gmail:
- League
- Teams
- Final score
- Match date

### ✔ 3. Weekly CSV Export
Every Sunday, the system exports all matches from the last 7 days into a CSV file and emails or uploads it.

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **Make.com** | Core automation engine |
| **OpenLigaDB API** | Sports data source |
| **Airtable** | Structured database |
| **Google Sheets** | Alternative database |
| **Gmail** | Notification system |

---

## 📊 Data Flow Diagram
OpenLigaDB API -> Make.com HTTP Module -> Iterator (loops through matches) -> Airtable / Sheets storage -> Router 1) Match finished → Gmail summary 2) Weekly scheduler → CSV export


## 📚 API Reference

🇩🇪 Bundesliga 1 (BL1)
https://www.openligadb.de/api/getmatchdata/bl1/2025

🇩🇪 Bundesliga 2 (BL2)
https://www.openligadb.de/api/getmatchdata/bl2/2025

🇩🇪 DFB Pokal
https://www.openligadb.de/api/getmatchdata/dfb/2025

🇪🇺 Champions League (CL)
https://www.openligadb.de/api/getmatchdata/cl/2023

🇪🇺 Europa League (EL)
https://www.openligadb.de/api/getmatchdata/el/2023

🇩🇪 Frauen-Bundesliga (Women)
https://www.openligadb.de/api/getmatchdata/fbl/2023

🏆 Euro Cup (National Teams)
https://www.openligadb.de/api/getmatchdata/em/2024

🏆 World Cup (National Teams)
https://www.openligadb.de/api/getmatchdata/wm/2022

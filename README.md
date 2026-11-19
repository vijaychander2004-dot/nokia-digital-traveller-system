Digital Traveller System: QR-based Repair Tracking for Nokia

Replacing the paper traveller sheet with one QR scan. Every telecom unit that comes in for repair is scanned at each station, updated digitally and synced in real time, so anyone can see its exact status and full history.



Built during my Winter Internship at Nokia Repair Centre, Gurgaon · Dec 2025 – Jan 2026

Digital Traveller home and auto-generated PDF traveller

🎬 Demo

▶ Watch the walkthrough · One-page write-up (PDF) · Presentation

The problem

Each Remote Radio Unit (RRU) that came in for repair travelled with a handwritten paper sheet. Fault details and repair status were often missing, unclear or damaged. Sheets got lost, units were hard to trace between stations, and technicians could not see where a unit stood. It also meant a lot of paper.

What I built

I spotted the problem while shadowing repair operations, proposed the fix to the Head of Repair Operations, and built it in three weeks:

QR printed on each RRU
Scan at station
Unit details auto-filled
Technician records result
Firebase real-time sync
Live dashboard / Power BI
Auto-generated PDFtraveller

Stations digitised: RC IN (scan & register) → Visual Inspection → RAP & Unit Test → Debug → Deep Tests → QC Check → Lot QC → Dashboard → Detach

Impact
No paper sheet: one digital record per unit, which no one can lose, smudge or misread.
Full traceability: one scan shows every station's result, the failures found, the parts replaced and the time taken.
Live status: supervisors see where each unit is and how many hours remain before its target date (10 days).
Less manual entry: scanning the QR fills in the serial number, product number, family and date and time automatically.
Shaped by users: reached v1.4.5 through feedback rounds with repair engineers. I presented it to senior engineers and the operations team, and they responded positively.
Key features
Checklists at each station (missing items, mechanical damage) with dropdowns and quick-add failure codes.
Pass/fail and retest logic for RAP, unit, TRX, PSU, OTA, LBTS, software and IP tests.
Module serial registration and a log of replaced components.
Turnaround tracking with a target date and a countdown of hours left.
Dashboard with status distribution and daily throughput, plus Excel export per station or for all data.
A one-click PDF Digital Traveller Sheet with a barcode, containing the unit's full repair lifecycle.
Tech stack

React · Firebase (real-time database) · QR/barcode scanning · Excel export · PDF generation · Power BI · hosted on the Repair Centre's local network

Screenshots
QR scan & register	Visual inspection
assets/screenshots/02_rc_in_qr_scan.jpg	assets/screenshots/03_visual_inspection.jpg
Final QC decision	Dashboard
assets/screenshots/04_final_qc.jpg	assets/screenshots/05_dashboard.jpg
My role

I identified the problem, proposed the solution, designed and built the app, collected feedback from engineers, and presented it to leadership. Alongside this, I built an automated attendance report in Power BI and Excel.

Vijay Chander · MSc Analytics, TISS Mumbai · vijaychander2004@gmail.com

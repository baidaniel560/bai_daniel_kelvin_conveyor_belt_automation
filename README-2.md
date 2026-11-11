# Automated Conveyor Belt Production and Fault Detection System

## Student Information
- **Name:** Bai Daniel Kelvin
- **Matric Number:** F/ND/24/3450011
- **Programme:** ND II Mechatronics Engineering
- **Institution:** Yaba College of Technology (YABATECH)
- **Course:** CTE213

## 1. Project Overview
This Python application is an educational simulation of a small industrial conveyor-belt production line. It models pre-start machine checks, product measurement and quality classification, production counting, and selected fault events.

The project focuses on industrial production and quality control. It is different from a smart water tank monitor, a workshop energy estimator, and a workshop tool inventory system.

## 2. Problem Statement
Production operators need reliable ways to count output, identify products outside required dimensions, and record machine faults. Manual inspection and record keeping can be inconsistent. This project demonstrates a simple digital approach to production monitoring and quality checks.

## 3. Aim and Objectives
**Aim:** To develop a Python simulation of a conveyor-belt production and fault detection process.

**Objectives:**
1. Simulate pre-start checks for an object sensor, motor status, and emergency stop.
2. Process a user-defined batch of products.
3. Classify products using dimensional tolerance.
4. Count accepted and rejected products.
5. Simulate motor over-temperature and conveyor jam alerts.
6. Keep production and fault histories.
7. Export records to CSV files.

## 4. Main Features
- Machine sensor inspection before a batch begins.
- Batch processing with a user-entered product count.
- Product quality check: accepted length is 9.5 cm to 10.5 cm.
- Automatic simulated reject decision for out-of-range products.
- Production totals and acceptance/rejection percentages.
- Motor over-temperature alert when the entered temperature exceeds 75°C.
- Simulated belt-jam event recording.
- Timestamped fault history.
- CSV export for production and fault records.

## 5. Python Concepts Demonstrated
- Variables and data types
- Functions
- Lists and dictionaries
- `for` and `while` loops
- Conditional statements (`if`, `elif`, `else`)
- User input and output
- Input validation and exception handling
- CSV file handling

## 6. Requirements
- Python 3.8 or later
- Terminal/command prompt or Python IDE
- No third-party packages required

## 7. How to Run
1. Download or clone this repository.
2. Open a terminal in the project folder.
3. Run:

   ```bash
   python conveyor_belt_system.py
   ```

4. Choose an option from the menu and follow the prompts.

## 8. Suggested Test Cases
| Test | Action | Expected result |
|---|---|---|
| Normal inspection | Sensor and motor `y`; emergency stop `n` | Inspection passes |
| Sensor fault | Sensor answer `n` | Fault logged; batch blocked |
| Product accepted | Enter 10.0 cm | Product accepted |
| Product rejected | Enter 11.0 cm | Product rejected |
| Motor over-temperature | Enter 80°C | Temperature fault logged |
| Belt jam | Answer `y` to obstruction prompt | Jam fault logged |
| Production report | Run a batch, then view report | Counts and percentages shown |
| CSV export | Select export option | Two CSV files created |

## 9. Limitations and Future Improvements
This is a classroom simulation and does not connect to a real conveyor, sensor, motor, relay, or PLC. Records are held in memory during the session; CSV export provides a copy for record keeping.

Future improvements could include database storage, a graphical interface, shift-based production targets, operator login, and connection to suitable hardware through a microcontroller or PLC.

## 10. Safety Note
This program is for educational demonstration only. It must not be used to operate or safeguard real industrial equipment. Real machinery requires properly engineered and tested hardware safety systems and qualified supervision.

## 11. Conclusion
The project demonstrates how Python can model a basic industrial automation workflow by combining machine checks, product quality inspection, production counting, fault logging, and report generation.

---
**Developed by:** Bai Daniel Kelvin  
**Matric Number:** F/ND/24/3450011  
**Course:** CTE213  
**Institution:** Yaba College of Technology (YABATECH)

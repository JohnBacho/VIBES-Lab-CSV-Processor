# CSV Eye-Tracking Processor

<div align="center">
<img width="400" alt="CSV Processor Logo" src="https://github.com/user-attachments/assets/89824d3a-373a-448f-9b5c-256f4c459466" />

<br>

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC--BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
[![JavaScript](https://img.shields.io/badge/Language-JavaScript-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Platform](https://img.shields.io/badge/Platform-Web-brightgreen.svg)](https://github.com/)
[![Status](https://img.shields.io/badge/Status-Development-orange.svg)]()
</div>


---

## 📖 Overview

**CSV Eye-Tracking Processor** is a lightweight JavaScript tool that reads raw eye-tracking CSV files and outputs cleaned, trial-averaged data ready for analysis.

This tool is designed to:

* Retain only the relevant columns (`Date`, `LocalTime`, `Phase`, `TrialNumber`, `Step`, `Stage`, `Context`, `leftEyePupilSize`, `rightEyePupilSize`, `GameObjectInFocus`)
* Calculate **average pupil size** per trial
* Compute **proportion of gaze on target objects**
* Generate cleaned CSV files with standardized naming based on hardware and experimental context

> ⚠️ Currently supports VR-based eye-tracking datasets (HTC VIVE Pro Eye) as well as tobii eye tracking files.

---

## 🛠️ Features

* **Column filtering** – Keep only the columns needed for analysis
* **Trial-based aggregation** – Computes trial averages for pupil size and gaze metrics
* **Context classification** – Automatically tags files as `AAA` or `ABA` based on experimental context
* **Automatic CSV download** – Outputs a processed CSV named `Program_[Hardware]_[ContextType]_DONE.csv`

---

## 📥 Usage

1. Open the HTML page that contains the script in your browser or [Link](https://johnbacho.github.io/VIBESLab-CSV-Formatter/)
2. Click the **file input** and select your raw CSV file.
3. The script will process the file automatically.
4. The cleaned CSV will download automatically to your machine.

> The script uses **JavaScript `FileReader`** and runs entirely in-browser—no server required.

---

## ⚙️ How It Works

1. Reads the CSV and splits it into rows and columns
2. Filters for only the relevant columns
3. Calculates:

   * **Average pupil size** per trial
   * **Proportion of gaze on objects of interest**
4. Handles baseline, instruction, and inter-trial rows
5. Generates a new CSV ready for analysis

---

## 👥 Core Team

| Name            | Major                      |
| --------------- | ------------------------- |
| John Bacho      | Computer Science            |
| Lauren Dunlap   | Computer Science       |
| Albert Selby    | Computer Science / Data Science              |
| Marissa Brigger | Neuroscience              |
| Alexa Gossett   | Neuroscience / Psychology |
| Jace Lander     | Software Engineer         |
| Corey Schwarz   | Computer Science / Data Science                |
| Cydney Hudson   | Neuroscience                |
| Olivia Mullins  | Neuroscience                |

---

## 📄 License

This project is licensed under **CC BY-NC 4.0**.

---

## 📧 Contact

* **Email:** [jbacho22@bw.edu](mailto:jbacho22@bw.edu)
* **Issues:** [GitHub Issues](https://github.com/YourUsername/CSV-EyeTracking-Processor/issues)

---

<div align="center">
Made with ❤️ by the VIBES Lab Team
</div>

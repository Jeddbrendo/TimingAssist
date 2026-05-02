# TimingAssist

# Timing Assistant

[![Made with HTML, CSS, JS](https://img.shields.io/badge/Made%20with-HTML%2C%20CSS%2C%20JS-blue.svg)](https://developer.mozilla.org/en-US/docs/Web)
[![PWA Ready](https://img.shields.io/badge/PWA-Ready-green.svg)](https://web.dev/progressive-web-apps/)


An offline-first, single-file web application designed to help plan and track meeting schedules with precision. This tool is built with vanilla JavaScript, is fully self-contained in a single HTML file, and leverages local storage to save your work automatically.

---

## ✨ Key Features

The Timing Assistant is divided into two powerful, purpose-built tabs:

### 1. Watchtower (WT) Timing Planner
A comprehensive scheduler for planning the Watchtower Study.

-   **Automatic & Manual Modes**: Quickly calculate average reading times or input granular paragraph-by-paragraph timings.
-   **CSV Import**: Instantly pre-fill the entire schedule by uploading a CSV file with paragraph durations. The importer is smart and can handle:
    -   Raw seconds (e.g., `170`).
    -   MM:SS format (e.g., `02:50`).
    -   Start and End times.
-   **Error Highlighting**: Any paragraph with a `0` second duration is automatically highlighted in red, alerting you to potential data errors.
-   **Live Schedule Generation**: Adjust any reading or comment time, and the entire schedule instantly recalculates.
-   **Print-Friendly Output**: A dedicated print view generates a clean, readable schedule perfect for the meeting.

### 2. CLM Time Tracker
A live stopwatch and variance tracker for the Christian Life and Ministry meeting.

-   **Live Time Tracking**: Use "Start" and "End" buttons to capture the exact time for each meeting part.
-   **Real-Time Variance**: Instantly see if a part is over or under its target time with color-coded variance pills.
-   **Dynamic Segments**: Add or remove parts from the "Living as Christians" section as needed for the week's schedule.
-   **Persistent State**: All your timings and configurations are saved locally in your browser.
-   **Shareable Reports**: Generate a clean, text-based report of the meeting's timing, perfect for copying into messages or notes.

---

## 🚀 How to Use

Simply download the `TimingAssist.html` file and open it in any modern web browser. No server or internet connection is required.

### Watchtower Timing Planner

1.  **Set Main Times**: Enter the meeting **Start Time** and **Finish Time**.
2.  **Choose Your Method**:
    -   **Automatic**: Enter the **Number of Paragraphs** and the **Total Audio Length** (MM:SS) from the official recording. The tool will calculate an average time for each paragraph.
    -   **Manual**: Check the **"Switch to Manual Time Entry"** box to input specific start/end times or reading durations for each paragraph.
    -   **CSV Import**:
        1.  Create a `.csv` file. The format can be simple or detailed. The importer will automatically detect the columns.
        2.  Click **"Choose CSV File"** and select your file. The schedule will be generated instantly.

**Sample CSV Formats:**

*Detailed (With Start/End Times)*
```csv
Paragraph,StartTime,EndTime,Duration
1,00:00,01:15,75
2,01:15,02:00,45
```

3.  **Generate Schedule**: Click **"Generate/Update Full Schedule"**.
4.  **Print**: Click **"Print Schedule"** for a clean, paper-friendly version.

### CLM Time Tracker

1.  **Configuration**: Set the meeting's official **Start Time**. The target end time will be calculated for you.
2.  **Live Tracking**: As the meeting progresses, click the **Start** and **End** buttons for each part.
    -   The live clock shows the current time.
    -   The variance pill `(Δ)` shows how close you are to the target.
3.  **Add/Remove Parts**: If there is an extra "Living as Christians" part, click **"Add Part"**. Use the delete icon to remove it.
4.  **Generate Report**: At the end of the meeting, click **"Share"**, select the details you want to include, and click **"Generate & Copy"** to copy the timing report to your clipboard.

---

## 🛠️ Technical Details

-   **Self-Contained**: The entire application lives in a single `TimingAssist.html` file. No dependencies, no frameworks.
-   **Vanilla JavaScript**: Built with pure JavaScript for maximum performance and portability.
-   **Local Storage**: Your data is automatically saved to your browser's local storage, so your timings persist between sessions.
-   **Progressive Web App (PWA) Ready**: Includes a manifest and icons, allowing you to "Add to Home Screen" on mobile devices for an app-like experience.
-   **Dark/Light Mode**: Both tabs feature a theme-switcher that respects your system preference and saves your choice.

---

# Spotify Listening Dashboard Excel Project

## 📊 Project Overview

This Excel-based dashboard provides a detailed and interactive exploration of my Spotify listening history, covering over **145,000** individual play events spanning multiple years. By meticulously cleaning, transforming, and analyzing the raw data, the dashboard uncovers meaningful patterns in listening behavior, skip habits, platform preferences, and temporal trends.

---

## 🔍 Data Description & Structure

- **Data Source**: Exported JSON/CSV from Spotify Playback History
- **Total Records**: 145,000+ rows (one row per playback event)
- **Key Columns**:
  - **Track Name**: Title of the song played
  - **Timestamp**: Date & time when playback started (ISO format)
  - **Artist**: Primary performing artist
  - **Album**: Album title associated with the track
  - **Timestamp**: Date & time when playback started (ISO format)
  - **Duration (min)**: Total duration of the track or podcast in minutes
  - **Platform**: Device used for playback (Mobile, Desktop, Web)

---

## 🧹 Data Cleaning & Preprocessing Steps

1. **Duplicate Removal**  
   - Identified and removed exact duplicate rows to ensure each playback event is unique.
2. **Integrity Checks**  
   - Filtered out records missing essential fields such as timestamp or track name.
3. **Timestamp Standardization**  
   - Converted all timestamps to a uniform datetime format in the system’s locale (Asia/Kolkata) to support consistent time-based analysis.
4. **Derived Metrics**  
   - **Playtime (minutes)**: Computed from duration for better readability.
   - **Skip Flag**: Marked events where a track was stopped before 30 seconds as a skip.
5. **Categorization**  
   - Mapped playback contexts into broader categories (e.g., Albums, Tracks, Artists etc.).

---

## 🔑 Key Analyses & Insights

### 1. Top Tracks, Artists & Albums
- **Top Tracks**: Ranked tracks by total play count and total playtime.
- **Top Artists**: Aggregated play counts by artist, revealing favorite musicians.
- **Top Albums**: Determined which albums saw the highest listening activity.

### 2. Total Listening Time
- **Cumulative Playtime**: Summed up total minutes listened per year and overall.
- **Average Session Length**: Calculated average listening duration per session.

### 3. Skip Behavior Analysis
- **Skip Rate**: Percentage of tracks skipped before 30 seconds.
- **Most Skipped Tracks**: Identified songs with the highest skip counts and skip ratios.
- **Skip Patterns**: Analyzed where within the track users most often give up (e.g., chorus, intro). Insights inform possible reasons for early exits.

### 4. Shuffle & Repeat Patterns
- **Shuffle Percentage**: Proportion of plays where shuffle mode was enabled.
- **Repeat Usage**: Frequency of single-track or album repeats.

### 5. Platform Usage Breakdown
- **Device Distribution**: Pie chart showing mobile vs. desktop vs. web usage.
- **Time-of-Day by Platform**: Heatmap indicating preferred platform by hour of day.

### 6. Temporal Trends
- **Day of Week Analysis**: Line graph of plays by weekday, highlighting peak listening days.

---

## 📊 Interactive Dashboard Components

1. **PivotTables & PivotCharts**  
   - Multi-level pivots for drilling into tracks, artists, albums, and time dimensions.
2. **Slicers & Timeline Controls**  
   - **Year Slicer**: Quickly filter data by year.
   - **Time Timeline**: Slide through months or quarters for fine-grained analysis.
3. **Dynamic KPIs & Cards**  
   - Total playtime, skip rate, shuffle percentage, and most-used platform update dynamically based on slicer selections.

---

## 🚀 Getting Started

1. **Download & Open**  
   - Open `Spotify_Dashboard.xlsx` in Microsoft Excel (2016 or later recommended).
2. **Enable Content**  
   - Enable data connections and external content if prompted to ensure full functionality.
3. **Refresh Data**  
   - After adding new raw data to the `RawData` sheet, go to **Data ➔ Refresh All** to update all PivotTables and charts.
4. **Interact**  
   - Use slicers and timeline controls on the `Dashboard` sheet to filter by year, day, or time period.
5. **Customize**  
   - Add or modify calculated fields in the PivotData model for further analysis.

---

## 📁 File Structure

```
Spotify_Dashboard/
├─ RawData.xlsx          # Exported Spotify data
├─ Spotify_Dashboard.xlsx # Main workbook with dashboard
├─ README.md            # Project documentation
└─ LICENSE              # MIT License details
```

---

## 🤝 Contributing & Feedback

Contributions, suggestions, and bug reports are welcome! Please open an issue or submit a pull request at:

```text
https://github.com/yourusername/spotify-dashboard-excel
```

---

## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for full terms.

---

*Documentation generated on April 23, 2025*


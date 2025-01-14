# Report: ISRO Mission Launch Dashboard Project

## 1. Project Overview

The ISRO Mission Launch Dashboard is an interactive web application designed to analyze and visualize data related to Indian Space Research Organisation (ISRO) satellite launches. The dashboard allows users to explore trends, applications, and orbit types associated with ISRO missions, offering insights through interactive charts and data tables.

---

## 2. Objectives

1. **Data Exploration**: To provide a comprehensive overview of ISRO’s satellite launches.
2. **Trend Analysis**: To identify yearly trends in the number of launches.
3. **Categorical Insights**: To categorize launches by application and orbit type.
4. **User Interaction**: To deliver a user-friendly, web-based interface for dynamic exploration of the dataset.

---

## 3. Tools and Technologies

- **Python**: Programming language for data processing and visualization.
- **Pandas**: For data manipulation and cleaning.
- **Streamlit**: Framework for building the interactive web-based dashboard.
- **Plotly**: Library for creating interactive visualizations.
- **VS Code**: Integrated Development Environment (IDE).

---

## 4. Dataset

The dataset used in the project is titled **"ISRO mission launches.csv"** and contains the following key columns:
- **Launch Date**: The date of the satellite launch.
- **Orbit Type**: The type of orbit for the mission.
- **Application**: The purpose of the satellite (e.g., Communication, Navigation).
- **Additional Metadata**: Other relevant details about the mission.

---

## 5. Folder Structure

```
ISRO_Dashboard_Project/
├── data/
│   └── ISRO mission launches.csv
├── isro_dashboard.py
├── requirements.txt
├── README.md
```

### File Descriptions:
1. **data/ISRO mission launches.csv**: The dataset used for analysis.
2. **isro_dashboard.py**: Main Python script containing the Streamlit dashboard logic.
3. **requirements.txt**: List of required Python packages.
4. **README.md**: Project documentation.

---

## 6. Data Preprocessing

### Steps:
1. **Loading Data**:
   - The dataset is loaded using Pandas.
   - Column names are standardized by removing extra spaces and replacing them with underscores.

2. **Data Cleaning**:
   - Conversion of `Launch Date` to datetime format.
   - Creation of a `Year` column for trend analysis.
   - Filling missing values in `Orbit Type` and `Application` columns with "Unknown."

3. **Validation**:
   - Verification of data types and removal of anomalies.

---

## 7. Dashboard Features

The Streamlit dashboard includes the following features:

### Sidebar:
- **File Upload**: Users can upload a CSV file for analysis.
- **Show Raw Data**: Toggle to display the raw dataset.

### Main View:
1. **Launches by Year**:
   - A bar chart showing the number of launches each year.
2. **Launches by Application**:
   - A pie chart categorizing launches by application.
3. **Launches by Orbit Type**:
   - A bar chart visualizing launches based on orbit type.

---

## 8. Visualizations

### 1. Launches by Year
- **Description**: Highlights the growth in ISRO’s launch capabilities over time.
- **Tool Used**: Plotly Bar Chart.

### 2. Launches by Application
- **Description**: Provides insights into the primary purposes of ISRO’s missions (e.g., Communication, Remote Sensing).
- **Tool Used**: Plotly Pie Chart.

### 3. Launches by Orbit Type
- **Description**: Displays the distribution of orbit types (e.g., GEO, LEO, MEO).
- **Tool Used**: Plotly Bar Chart.

---

## 9. Running the Project

### Prerequisites:
1. Install Python (>= 3.8).
2. Install required libraries using:
   ```bash
   pip install -r requirements.txt
   ```

### Steps:
1. Navigate to the project directory:
   ```bash
   cd ISRO_Dashboard_Project
   ```
2. Run the Streamlit app:
   ```bash
   streamlit run isro_dashboard.py
   ```
3. Open the dashboard in your browser and upload the dataset.

---

## 10. Insights

1. **Trends Over Time**:
   - A consistent increase in the number of launches reflects ISRO’s growing capabilities.
2. **Applications**:
   - Communication and Remote Sensing dominate as primary applications.
3. **Orbit Types**:
   - Low Earth Orbit (LEO) is the most commonly targeted orbit.

---

## 11. Challenges and Solutions

### Challenges:
- Handling missing values in key columns.
- Ensuring the dashboard is responsive and user-friendly.

### Solutions:
- Used default values for missing data (e.g., "Unknown").
- Optimized visualizations with Plotly for interactivity.

---

## 12. Future Enhancements

1. **Additional Data Sources**:
   - Integrate real-time data from APIs.
2. **Advanced Analytics**:
   - Perform predictive analysis on launch trends.
3. **Export Feature**:
   - Add an option to export visualizations and reports.

---

## 13. Conclusion

The ISRO Mission Launch Dashboard effectively visualizes ISRO’s satellite launch data, providing insights into trends, applications, and orbit types. This project demonstrates the power of data visualization and serves as a foundation for more advanced space mission analytics.

---

## 14. References

- [ISRO Official Website](https://www.isro.gov.in)
- Streamlit Documentation
- Pandas Documentation
- Plotly Documentation

## Name:- Chandra Sekhar Potturi

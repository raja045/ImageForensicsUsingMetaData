# ImageForensicsUsingMetaData

# Image Forensics Using Metadata

## Project Overview
This project focuses on utilizing metadata to enhance image forensics. Metadata provides critical insights into the origin, authenticity, and context of images, making it a powerful tool in criminal investigations. By automating metadata extraction and anomaly detection, this project addresses the challenges of manual metadata analysis, which is often time-consuming and error-prone.

---

## Objectives
1. **Metadata Extraction**: Extract technical and contextual information from images.
2. **Anomaly Detection**: Leverage machine learning to identify suspicious patterns.
3. **Geospatial Visualization**: Use visualization tools to effectively represent metadata insights.

---

## Problem Statement
Manual analysis of metadata is prone to errors and inefficiencies. This project automates:
- Extraction of critical metadata fields such as GPS, timestamps, and camera details.
- Detection of anomalies using machine learning.
- Geospatial visualization of metadata insights.

---

## Methodology
### 1. Metadata Extraction
- **Tool Used**: ExifRead Python Library.
- **Extracted Fields**:
  - GPSInfo: Geolocation data (latitude, longitude, altitude).
  - DateTimeOriginal: Timestamp of the original capture.
- **Output**: Structured metadata for analysis.

### 2. Anomaly Detection
- **Model Used**: Isolation Forest.
- **Detection Criteria**:
  - **Time Difference**: Abnormal creation and modification intervals.
  - **Geospatial Information**: Inconsistent GPS data.
  - **File Size**: Deviations indicating editing or compression.
  - **Date Shot**: Irregular shooting times.

### 3. Geospatial Visualization
- **Tools Used**:
  - **Matplotlib** & **Seaborn**: Data plots.
  - **Folium**: Interactive maps for GPS data.

---

## Technologies Used
- **Programming Language**: Python.
- **Libraries**:
  - ExifRead for metadata extraction.
  - Scikit-learn for anomaly detection.
  - Pandas & NumPy for data analysis.
  - Matplotlib, Seaborn, & Folium for visualization.

---

## Dataset
The final dataset includes the following columns:
- File
- Date Shot
- Date Created
- Date Modified
- Latitude
- Longitude
- Device
- File Size (KB)
- Resolution
- Time Difference (Days)
- Anomaly

---

## Key Results
### Types of Anomalies Detected
1. **Time Gaps**: Abnormal modification intervals (highlighted with red lines).
2. **Out-of-Sequence Events**: Suspicious timeline inconsistencies.
3. **Location Inconsistencies**: Mismatched GPS data.

### Visual Representations
![Time Gaps](images/time_gaps.png)  
![Location Anomalies](images/location_anomalies.png)

---

## Conclusion
The project successfully demonstrated how metadata extraction, anomaly detection using Isolation Forest, and visualization can streamline image forensics. This approach enhances the ability to validate evidence, identify tampering, and provide actionable insights in forensic investigations.

---

## References
1. Sagnik Ray Choudhury et al. “Figure Metadata Extraction from Digital Documents”. In: *12th International Conference on Document Analysis and Recognition* (2013).
2. Runtao Liu et al. “Automatic Document Metadata Extraction Based on Deep Networks”. In: *Natural Language Processing and Chinese Computing* (2018).
3. MA Manso et al. “Automatic metadata extraction from geographic information”. In: *7th Conference on Geographic Information Science* (2004).
4. Caleb Riggs et al. “Image Mapping through Metadata”. In: *3rd International Conference on Security of Smart Cities, Industrial Control System and Communications* (2018).
5. Evagelos Varthis et al. “Automatic metadata extraction via image processing using Migne’s Patrologia Graeca”. In: *International Journal of Metadata, Semantics and Ontologies* (2020).
 


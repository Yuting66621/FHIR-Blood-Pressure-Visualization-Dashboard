# FHIR Blood Pressure Visualization Dashboard

## Overview
This dashboard visualizes blood pressure data using the FHIR API and Highcharts library. It displays the blood pressure trends for a specific patient over time.

## Patient Information
- **Patient ID**: `d2fd4a58-b2c1-4078-ae3f-8ccdc5430bea`

## Data Source
The dashboard retrieves blood pressure observations using the FHIR API from the SMART Health IT sandbox:

**API Endpoint**:
```
https://r3.smarthealthit.org/Observation?code=http://loinc.org|55284-4&_sort=date&patient=d2fd4a58-b2c1-4078-ae3f-8ccdc5430bea
```

**LOINC Code**: `55284-4` (Blood Pressure)

## Data Structure
The blood pressure observation contains two components:
1. **Systolic** - The pressure when the heart beats (component[0])
2. **Diastolic** - The pressure when the heart rests between beats (component[1])

## Visualization
The dashboard presents a line chart showing:
- **X-axis**: Date of observation
- **Y-axis**: Blood pressure values in mmHg
- **Two lines**: One for systolic pressure and one for diastolic pressure

This allows users to track blood pressure changes over time and identify trends.

## Technologies Used
- **FHIR Client Library**: For accessing healthcare data via FHIR API
- **Highcharts**: For creating interactive data visualizations
- **SMART Health IT**: Test FHIR server (R3)

## How to Use
Simply open the HTML file in a web browser. The dashboard will automatically fetch and display the patient's blood pressure data.

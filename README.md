# Data Intelligence Automation with AI-Enhanced Visuals

## **Project Overview**
This project automates the process of analyzing data, creating visualizations, and generating insights from any given CSV dataset. It leverages the capabilities of GPT-4o-Mini and cutting-edge data processing tools to produce detailed Markdown reports with accompanying visualizations. Designed for flexibility, the system is compatible with a wide range of datasets, providing thorough analysis and actionable insights.

---

## **Key Features**
1. **Complete Automated Data Analysis**  
   - Computes summary statistics, identifies missing data, and flags anomalies.
   - Performs correlation and clustering analyses to uncover underlying patterns.
   - Uses GPT-4o-Mini to offer advanced insights, analysis suggestions, and method refinements.

2. **Dynamic Visualization Creation**  
   - Automatically generates 1–3 informative charts (in PNG format) customized for each dataset.
   - Supports a variety of visualizations such as heatmaps and bar graphs.

3. **Insightful Narrative Generation**  
   - GPT-4o-Mini generates detailed descriptions of datasets, analysis methods, and findings.
   - Produces a unified Markdown report that integrates both the analysis and visual content.

4. **Optimized Use of LLM Resources**  
   - Minimizes direct dataset transfer by preprocessing the data before sending it to the LLM.
   - Optimizes token usage, ensuring comprehensive analysis without compromising precision.

5. **Broad Compatibility with CSV Datasets**  
   - Adapts to different dataset types and structures, ensuring strong and scalable performance across varied data formats.

6. **Independent and Standalone Execution**  
   - The project runs as a single script (`autolysis.py`), with no external dependencies beyond basic Python libraries.

7. **Simple Integration and Usage**  
   - Run the analysis with a single command through the `uv` CLI tool:
     ```bash
     uv run autolysis.py dataset.csv
     ```

---

## **Workflow**
1. **Data Preprocessing**  
   - Extracts essential metadata from the CSV file, including column names, types, and sample values.
   - Detects missing values, anomalies, and potential outliers for further analysis.

2. **Exploratory Data Analysis (EDA)**  
   - Performs statistical summaries, correlation analysis, anomaly detection, and clustering techniques.

3. **Integration with GPT-4o-Mini**  
   - Sends metadata and EDA results to GPT-4o-Mini for further insights and additional analytical suggestions.

4. **Creation of Visualizations**  
   - Generates charts using **Seaborn** and **Matplotlib** libraries, storing the resulting PNG files for easy access.

5. **Report Generation**  
   - GPT-4o-Mini creates a structured Markdown report containing:
     - Overview of the dataset
     - Analysis techniques employed
     - Major findings and their implications
     - Visual representations of the results

6. **Output Files**  
   - `README.md`: Comprehensive Markdown report.
   - PNG files: Charts and visualizations in PNG format.

---


## **Usage Instructions**
1. **Set the authentication token:**
   ```bash
   export AIPROXY_TOKEN=your-token-here
## **Technical Notes**

### **Optimized LLM Utilization**
- The system employs multiple queries to the LLM to conduct detailed analyses and provide visualization recommendations.
- Integrates OpenAI’s function-calling API for improved precision and efficient data processing.

### **Environment Configuration**
- Requires the `AIPROXY_TOKEN` environment variable for authenticating the LLM.

### **Visualization Tools**
- Utilizes libraries such as **Seaborn** and **Matplotlib** to create compelling, insightful visualizations that are automatically generated and saved as PNG files.

---

## **Deliverables**

### **Core Python Script:**
- `autolysis.py`: A standalone Python script that encapsulates all functionalities for automated data analysis and reporting.

### **Generated Output Files:**
- Separate directories for each dataset (e.g., `goodreads/`, `happiness/`, `media/`) containing:
  - `README.md`: The comprehensive Markdown report.
  - `*.png`: Visualization files in PNG format.

---

## **Licensing**
This project is licensed under the **MIT License**. For more details, refer to the `LICENSE` file in the repository.

---

This project exemplifies the integration of advanced analytical techniques with LLM-powered insights, offering both technical rigor and practical value. Explore the power of automated data analysis and visualization!


# DataEngineeringCourse3Lab2

ETL data from different files csv,xml,json

## Requirements

* Python 3.x
* pandas
* xml.etree.ElementTree
* glob

## Usage

1. Ensure you have the required Python packages installed.
2. Place your CSV, JSON, and XML files in the same directory as the script.
3. Run the script.

## Functions

### 1. `extract_from_csv(file_to_process)`

This function extracts data from a CSV file and returns it as a pandas DataFrame.

### 2. `extract_from_json(file_to_process)`

This function extracts data from a JSON file and returns it as a pandas DataFrame.

### 3. `extract_from_xml(file_to_process)`

This function extracts data from an XML file and returns it as a pandas DataFrame.

### 4. `extract()`

This function orchestrates the extraction process by iterating through all CSV, JSON, and XML files in the directory and combining the extracted data into a single DataFrame.

### 5. `transform(data)`

This function transforms the extracted data by converting height from inches to meters and weight from pounds to kilograms.

### 6. `load_data(target_file, transformed_data)`

This function loads the transformed data into a target CSV file.

### 7. `log_progress(message)`

This function logs progress messages with timestamps to a log file (`log_file.txt`).

## Running the Script

1. The script initializes by logging the start of the ETL job.
2. It then extracts data from CSV, JSON, and XML files, logging the start and end of the extraction phase.
3. Next, it transforms the extracted data, converting measurements and logging the start and end of the transformation phase.
4. Finally, it loads the transformed data into a CSV file and logs the start and end of the loading phase.
5. The script concludes by logging the end of the ETL job.

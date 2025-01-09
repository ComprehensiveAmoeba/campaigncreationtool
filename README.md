# Amazon Campaign Creation Tool

## Overview
The Amazon Campaign Creation Tool is a Streamlit-based application that allows users to generate customized advertising campaigns for Amazon Sponsored Products. The tool simplifies campaign creation by validating input data, generating campaign files, and providing downloadable outputs.

## Features
- **Input Validation**: Ensures that data in the input CSV meets required specifications (e.g., ASIN format, daily budget limits).
- **Dynamic Campaign Name Generation**: Supports naming conventions based on match type and user-defined tags.
- **Cross Negation Option**: Allows users to manage keyword cross-negation for broad and phrase match campaigns.
- **Quartile Management**: Adds the prefix `UN_` to campaign names for unmanaged quartiles based on user input or a CSV column.
- **Downloadable Outputs**: Generates an Excel file with all campaign details.

## Instructions

1. **Prepare the Input File**:
   - Use the [template](https://docs.google.com/spreadsheets/d/1EfaegRfxOOclnPptF2u5xnLvylG634mQKqwqXQDMfcg/edit?gid=0#gid=0) and download it as a CSV.
   - Ensure all required columns are filled and follow the format described in the template.

2. **Upload the CSV File**:
   - Click on the "Choose a CSV file" button to upload your prepared input file.

3. **Select Options**:
   - **Cross Negation**: Choose whether to apply keyword cross-negation for broad and phrase match campaigns.
   - **All Quartile Unmanaged**: Check this box to mark all campaigns as unmanaged, overriding the `Unmanaged by Quartile?` column in the input.

4. **Generate Campaign File**:
   - Click the "Generate Campaign File" button to create the campaign output.
   - If any validation errors are found, download the error report, correct the issues, and re-upload the CSV.

5. **Download the Output**:
   - Once generated, download the campaign file in Excel format.

## Requirements
- Python 3.7+
- Required packages (see `requirements.txt`):
  - `streamlit`
  - `pandas`
  - `openpyxl`

## Setup

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:
   ```bash
   streamlit run app.py
   ```

4. Access the app in your browser at `http://localhost:8501`.

## File Structure
- `app.py`: Main application script.
- `requirements.txt`: List of dependencies.

## License
This project is licensed under the MIT License.

---

If you encounter any issues or have feature requests, feel free to open an issue or contribute to the project!

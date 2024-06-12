# DICOM Header Extractor

This project extracts DICOM headers, de-identifies specific tags, and saves the information to a CSV file.

## Requirements

To run this project, you need the following libraries:
- DCM4CHE library (https://github.com/dcm4che/dcm4che)

## Usage

1. Compile the Java code:
    ```bash
    javac Main.java HeaderInfo.java DicomElement.java DicomReader.java
    ```

2. Run the program:
    ```bash
    java Main --directory /path/to/your/directory --deidentify
    ```

The `output.csv` file will be generated in your working directory.

## References

The DICOM tags selected for de-identification in this project are based on the following paper:
- Aryanto KYE, Oudkerk M, van Ooijen PMA. Free DICOM de-identification tools in clinical research: functioning and safety of patient privacy. Eur Radiol. 2015;25(12):3685-3695. doi:10.1007/s00330-015-3794-0

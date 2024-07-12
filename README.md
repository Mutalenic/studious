# Malware and Corruption Scanner

This repository contains a Python script designed to scan files for malicious signatures (using the EICAR test file) and check for file corruption based on an expected signature.

## Features

- **Malicious File Detection**: Identifies files containing a specific malicious signature.
- **File Corruption Check**: Verifies if files are corrupted based on a predefined signature.
- **Directory Scanning**: Recursively scans directories for malicious and corrupted files.

## Prerequisites

- Python 3.x
- Basic understanding of Python and file systems.

## Getting Started

### Clone the Repository

git clone https://github.com/Mutalenic/studious.git
cd studious


### Position the EICAR Test File

1. **Download the EICAR test file**: You can download the EICAR test file from [here](https://www.eicar.org/download/eicar-com-2/).
2. **Place the file**: Move the downloaded `eicar.com` file to `C:\Users\USER\Desktop\ME\eicar.com`.

### Modify the Script

1. **Open the script**: Open `malware.py` in a text editor.
2. **Change the file path**:
   - Locate the following line in the script:
          single_file_path = r"C:\Users\USER\Desktop\ME\eicar.com"
   - If your `eicar.com` file is in a different location, update the path accordingly.

### Running the Script

1. **Open Terminal/Command Prompt**:
   - **Windows**: Press `Win + R`, type `cmd`, and press `Enter`.
   - **Mac/Linux**: Open the Terminal application.

2. **Navigate to the Script Directory**:
   - Use the `cd` command to navigate to the directory where you cloned the repository.
   - Example:
          cd path\to\malware-corruption-scanner
     
3. **Run the Script**:
   
   python malware.py
   

## Script Output

- **File not found**: If the script cannot find the `eicar.com` file, ensure the file path is correct.
- **Malicious file detected**: If the script detects the malicious signature, it will prompt you to delete the file.
- **File is not corrupted**: If the file matches the expected signature, it is not corrupted.
- **File may be corrupted**: If the file does not match the expected signature, it may be corrupted.

## Customizing the Script

### Change Directory to Scan

- Locate the following line in the script:
    target_directory = r"C:\dev"
- Update the path to the directory you want to scan.

### Change Expected Signature

- Locate the following line in the script:
    expected_signature = b"GIF89a"
  - Update the expected signature based on the type of files you are scanning.

## Contribution

Feel free to fork the repository and submit pull requests for any improvements or additional features you would like to add.

## License

This project is licensed under the MIT License.
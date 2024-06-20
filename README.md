# Package Checker Script
By irvin cardoza

This repository contains `script.py`, a script designed to make downloading and managing Python packages easier by comparing the currently installed packages with those specified in `requirements.txt`.

## Overview

The `script.py` script takes the output of the `pip list` command as input, processes this data, and compares the installed packages with the ones listed in `requirements.txt`. It then identifies any missing packages or version mismatches and provides an easy way to install the missing packages by generating the appropriate `pip install` commands.

## Features

- The script reads the list of installed packages and their versions from the `pip list` output and compares them to the packages listed in `requirements.txt`.
  
- It identifies packages that are listed in `requirements.txt` but are not installed in the current environment.
  
- The script also checks for version mismatches, ensuring that the installed versions of the packages match those specified in `requirements.txt`.
  
- For each missing package or version mismatch, the script generates a `pip install` command that the user can simply copy and paste into the terminal to install the required packages.

## Usage

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/irvincardoza/installation-script.git
   
    ```

2. **Prepare the `requirements.txt` File**:
    Ensure you have a `requirements.txt` file in the repository. This file should list all the required packages and their versions.

3. **Run the Script**:
    Execute `script.py` and provide the `pip list` output when prompted.
    ```bash
    python script.py
    ```

4. **Paste the `pip list` Output**:
    When prompted, paste the output of the `pip list` command and press Enter twice.

5. **Review Missing Packages**:
    The script will output a list of missing packages and version mismatches along with `pip install` commands for easy installation.

## Example

```bash
Please paste your 'pip list' output below and then press Enter twice when done:

wheel                             0.41.2
widgetsnbextension                3.5.2
wrapt                             1.14.1
wurlitzer                         3.0.2
...

Missing packages:
pip install numpy==1.21.0
pip install pandas==1.3.0
pip install scipy==1.7.0
...
```
All you need to do is copy and paste these commands into your terminal to install the missing packages.

## Contributing

Feel free to open issues or submit pull requests if you have suggestions for improvements or if you encounter any bugs.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

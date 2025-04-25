# Zinc Downloader
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\
Zinc Database Downloader &amp; Merger

Due to the Zinc15 & Zinc20 database website's limitations on downloading big dataset files in .sdf, .smi & other formats, this tool will help you to easily download any dataset you want based on your zinc ID's list file.

## Prerequired Python libraries:
* requests
* colorama
* tqdm

## Prerequiered files:
Zinc ID's list:\
To create your Zinc ID's list you can download the CSV file of your preferred dataset and convert it to a list TXT file or create the list TXT file manually. Be aware that the Zinc ID's list file must be created in .txt format. For more information on how the final file has to be you can take a look at the [list.txt](list.txt) file existing in the project files.

## How to Run:
1. Confirm Requirements Installation
***Make sure the following are installed:
   ```
   pip install requests tqdm colorama

2. Prepare Input File
The script expects a file (default: list.txt) with ZINC IDs listed line by line:
```
ZINC000001
ZINC000002
ZINC000003
```
3. Run the Script
Use the command line to execute the script:
```
python zinc_downloader.py
```
4. Follow the interactive prompts:

Zinc version:
```
15 or 20
```
File type: 
```
choose from sdf, smi, csv, xml, json
```
Input file: 
```
press Enter to use list.txt, or type a custom file
```

Merge?: type yes if you want all downloaded files merged into one


## Final outputs:
The script creates two separate folders in its related folder at the end:
### 1.
```
dataset
```
which contains all downloaded dataset molecules
### 2.
```
merged_dataset
```
which contains one molecule created by merging molecules in the dataset folder

## Contact:
For further support and any questions, you can contact me via:

[![Static Badge](https://img.shields.io/badge/Telegram%20-%20shadmehr_gh%20-%20blue?style=flat&logo=telegram&color=blue)](https://t.me/shadmehr_gh)\
[![Static Badge](https://img.shields.io/badge/Gmail%20-%20shadmehr.ghorbani78%40gmail.com%20-%20red?style=flat&logo=gmail)](mailto:shadmehr.ghorbani78@gmail.com)\
[![Static Badge](https://img.shields.io/badge/Academic%20Email%20-%20sh--ghorbani%40student.tums.ac.ir%20-%20silver?style=flat)](mailto:sh-ghorbani@student.tums.ac.ir)\
[![Static Badge](https://img.shields.io/badge/Linkedin%20-%20shadmehr--ghorbani%20-%20blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/shadmehr-ghorbani)\
[![Static Badge](https://img.shields.io/badge/Researchgate%20-%20shadmehr--ghorbani%20-%20green?style=flat&logo=researchgate)](https://www.researchgate.net/profile/Shadmehr-Ghorbani)



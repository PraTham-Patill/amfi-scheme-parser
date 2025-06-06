# amfi-scheme-parser

# AMFI Scheme Name and Asset Value Extractor

This repository contains a shell script that extracts the **Scheme Name** and **Asset Value** from the official AMFI (Association of Mutual Funds in India) data file and saves it as a **TSV (Tab-Separated Values)** file.

## 📄 Source
Data is fetched from: [https://www.amfiindia.com/spages/NAVAll.txt](https://www.amfiindia.com/spages/NAVAll.txt)

## 📜 Script
The shell script performs the following:
- Downloads the NAVAll.txt file using `curl`
- Extracts only the **Scheme Name** and **Asset Value** fields using `awk`
- Saves the output in a `.tsv` file

## 🔧 Requirements
- Unix-based terminal
- curl
- awk

## 🚀 Usage
```bash
bash amfi_parser.sh
```
This will create a file named `amfi_data.tsv` in the same directory.

## 📁 Output Format (TSV)
```
Scheme Name	Asset Value
Scheme 1	123.4567
Scheme 2	234.5678
...
```

## ❓ Should this data be in JSON?
If the goal is to visualize, share, or process data in spreadsheets, TSV is perfectly fine. However, **JSON** is more suitable for **web applications, APIs, or structured programmatic access** where key-value representation offers more flexibility and integration potential.

## ✍️ Author
Pratham Patil

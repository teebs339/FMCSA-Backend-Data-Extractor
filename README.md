# FMCSA Backend Data Extractor

[![UiPath](https://img.shields.io/badge/UiPath-RPA-blue)](https://www.uipath.com/)
[![Excel](https://img.shields.io/badge/Excel-Macros-green)](https://www.microsoft.com/en-us/microsoft-365/excel)

This project is an **RPA bot built with UiPath** that extracts backend data from [ai.fmcsa.dot.gov](https://ai.fmcsa.dot.gov/) for different trucking LLCs.

It uses **HTTP requests** to pull company data, applies **RegEx** to parse and transform the raw HTML into a human-readable format, and outputs the results into a neat **Excel report**.

A built-in **VBA script** automatically applies formatting to the final Excel file, so you get a polished report out of the box.

## Features

* Automates data retrieval from FMCSA backend.
* Parses and cleans data with **regular expressions**.
* Generates a formatted **Excel report** with VBA styling.
* Simple input file structure for easy customization.

## Requirements

* [UiPath Studio](https://www.uipath.com/) installed on your machine.
* Microsoft Excel with macros enabled.

---

## Setup & Installation

1. **Clone this repository**

   ```bash
   git clone https://github.com/teebs339/FMCSA-Backend-Data-Extractor.git
   cd FMCSA-Backend-Data-Extractor
   ```

2. **Enable Excel macros**

   * Open Excel.
   * Go to:
     `File > Options > Trust Center > Trust Center Settings > Macro Settings`
   * Select **Enable all macros**.
   * Check **Trust access to the VBA project object model**.

3. **Open the project in UiPath Studio**

   * Launch UiPath Studio.
   * Open the project folder you just cloned.

## Usage

1. In the **Input** folder, open `Input.xlsx`.
2. Replace the sample values in the **MX Number** column with your own MX Number(s) or US DOT Number(s).

   * You may remove the other sample columns if not needed.
3. Run the bot in UiPath.
4. Once completed, the bot will generate `Report.xlsx` inside the **Output** folder, formatted and ready to use.

## Contributing

Feel free to **fork this repo**, suggest improvements, or open issues.
If you have questions, drop a message in the discussions section.

## Disclaimer

This project uses public FMCSA data. Please ensure your use complies with FMCSA’s [data policies](https://www.fmcsa.dot.gov/registration/fmcsa-data-disclaimer) and terms of service.

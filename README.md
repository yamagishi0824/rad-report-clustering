# Japanese Radiology Report Information Extraction and Clustering

This repository contains two Jupyter notebooks that demonstrate how to extract structured information from radiology reports using large language models (LLMs) and subsequently cluster the extracted information for further analysis.

## Repository Structure

- `notebooks/1_information_extraction_using_llm.ipynb`:  
  This notebook focuses on extracting structured data from radiology reports using LLMs. It demonstrates the process of preparing prompts, generating outputs in JSON format, and saving the results for downstream applications.

- `notebooks/2_clustering_extracted_infomation.ipynb`:  
  This notebook analyzes the structured data extracted from the radiology reports. It demonstrates clustering methods to identify patterns or group similar information.

## Requirements

To run the notebooks, you will need the following:
- Python 3.8 or later
- Required libraries: `pandas`, `torch`, and any additional libraries specified in the notebooks.

Install dependencies using:
```bash
pip install -r requirements.txt
```

## Usage

1. Place your radiology report data in a CSV file, ensuring that:
   - For `1_information_extraction_using_llm.ipynb`, the CSV file has a column named `text` containing the radiology reports.
   - For `2_clustering_extracted_infomation.ipynb`, the input CSV file has a column named `text_json` with structured data in JSON format.

2. Run the notebooks in the specified order:
   - Start with `1_information_extraction_using_llm.ipynb` to extract structured information.
   - Proceed with `2_clustering_extracted_infomation.ipynb` to analyze and cluster the extracted data.

## Example Data

Sample CSV files for input and output formats:
- Input for extraction: `data/reports.csv`
- Output for clustering: `data/extracted_info.csv`

Ensure that the appropriate file paths are updated in the notebooks before running.

## License

This project is released under the MIT License. Feel free to use, modify, and share.

## Citation

Coming soon...

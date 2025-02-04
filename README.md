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

This repository's code is licensed under the MIT License. You are free to use, modify, and distribute this code as permitted by the terms of the MIT License.
Please note that this project relies on third-party libraries and models (e.g., PyTorch, transformers), which may have their own licensing terms. By using this repository, you agree to comply with the licenses of any dependencies or models included or referenced in this project.

## Citation

```
@article{yamagishi2025llmcl,
  title     = {Large Language Model Approach for Zero-Shot Information Extraction and Clustering of Japanese Radiology Reports: Algorithm Development and Validation},
  author    = {Yamagishi, Y and Nakamura, Y and Hanaoka, S and Abe, O},
  journal   = {JMIR Cancer},
  volume    = {11},
  pages     = {e57275},
  year      = {2025},
  doi       = {10.2196/57275},
  url       = {https://cancer.jmir.org/2025/1/e57275}
}
```

# HTML to Markdown Conversion Notebook

This repository contains a small Python utility implemented as a Jupyter notebook
that converts a webpage into a Markdown file.

## What it does

The notebook:
- Downloads a webpage using HTTP
- Converts the HTML content into Markdown
- Saves the result as a local text file

This is useful for:
- Archiving web-based guidance
- Creating offline-readable documentation
- Preparing content for version control or review

## Requirements

- Python 3
- Jupyter Lab or Jupyter Notebook

Python packages used:
- `requests`
- `html2text`

All dependencies are installed directly within the notebook.

## How it works

1. A URL is retrieved using `requests`
2. The HTML is converted to Markdown using `html2text`
3. The Markdown output is written to a local file path

The main logic is contained in two functions:
- `url_to_markdown(url)`
- `save_website_as_MD(urlAddress, outputPath)`

## Usage

1. Open the notebook in Jupyter Lab or Jupyter Notebook
2. Update the `urlAddress` and `outputPath` variables if required
3. Run all cells

The final cell performs the conversion and saves the output file.

## Notes

- Output quality depends on the source website’s HTML structure
- The notebook does not remove navigation, headers, or embedded elements
- Best results are achieved with content-heavy, text-focused webpages

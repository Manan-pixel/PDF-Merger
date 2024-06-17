# PDF-Merger

This Python script allows you to merge multiple PDF files into a single PDF file. The script uses the `PyPDF2` library to handle PDF manipulation.

## Requirements

- Python 3.x
- `PyPDF2` library

You can install the required library using pip:

```bash
pip install PyPDF2
```

## Usage

1. **Clone the Repository**

2. **Set the paths**

   Modify the script to include the paths of the PDFs you want to merge and the output file name. Example:

   ```python
   files_list = [
       "/content/part1.pdf",
       "/content/part2.pdf"
   ]
   output_file = "/content/merged_output.pdf"
   ```

3. **Run the Script**

   ```bash
   Run the Entire Program
   ```

4. **Merged PDF**

   The merged PDF will be saved with the name specified in the `merged_output` variable.

## Script Explanation

### PdfWriter Function

- PdfWriter is used to write the merged PDF file.
- PdfReader is used to read each input PDF file.

- files_list is a list of file paths for the PDFs that will be merged. Adjust these paths to match your files.
- output_file is the path where the merged PDF will be saved.
- An instance of PdfWriter is created to manage the merged PDF file.
- The script iterates over each PDF file in files_list.
- Each file is read using PdfReader.
- All pages from each file are added to PdfWriter.
- The merged PDF content is written to output_file using a context manager to ensure the file is properly closed after writing.


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

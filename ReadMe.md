# CheckBoxOCR

A CLI tool to detect checked and unchecked checkboxes from PDFs and images.

---

## How to use
Run the executable from the `CheckBoxOCR` folder with your file as an argument:

```bash
./CheckBoxOCR/ocr yourfile.pdf
```

On Windows:

```cmd
CheckBoxOCR\ocr.exe yourfile.pdf
```

Supported input file types:

- Documents (.pdf)  
- Images (.png, .jpg, .jpeg, .bmp)

---

## Output

- Annotated images with detected checkboxes saved in the `output/` folder (This will be automatically generated for you on first run)
- Console output lists checkbox statuses and their positions on each page

---

## Integration
(c.pdf is a sample pdf file to ensure the model runs)

You can integrate this tool into your own automation or pipelines by calling the binary directly.
(Replace yourfile.pdf with the image or PDF you want to use)
Example (shell):

```bash
./CheckBoxOCR/ocr yourfile.pdf 
```

Example (Python):

```python
import subprocess
subprocess.run(["./CheckBoxOCR/ocr", "yourfile.pdf"])
```

This makes it easy to include checkbox detection in document processing systems or form analysis flows.

---

This is a packaged tool, there is no need to install any other packages. 

Any Problems? Feel free to raise them via the issues tab.
Improvements in the model will be released bi-monthly.  

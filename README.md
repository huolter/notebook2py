# Notebook2Py
### Effortlessly convert your Jupyter notebooks into Python scripts!

## Features:

* Extracts code cells from Jupyter notebooks.
* Preserves code execution order.
* Adds a header comment indicating the source notebook (optional).

## Example ussage:

```python
# Import the notebook_to_python function
from notebook2py import notebook_to_python

# Set the notebook and output filenames
notebook_file = "notebook1.ipynb"

# Convert the notebook using the default settings
output_file = notebook_to_python(notebook_file)
print(f"Successfully converted {notebook_file} into {output_file}!")

# Convert the notebook with a name change
output_file = notebook_to_python(notebook_file, "another_name.py")
print(f"Successfully converted {notebook_file} into {output_file}!")
```

:-)

 s
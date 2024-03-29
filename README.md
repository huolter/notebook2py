# Notebook2Py
### Effortlessly convert your Jupyter notebooks into Python scripts!

## Features:

* Extracts code cells from Jupyter notebooks.
* Preserves code execution order.
* Adds a header comment indicating the source notebook (optional).

To start using it just copy the notebook2py.py script to your root and import notebook_to_python. 

Also, check the example/ folder in this repo. 

## Simple example ussage:

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

## How I use it:

I like to code in notebooks, and I am using this solution to incorporate the notebook_to_python pipeline of all my notebooks, and then
call functions that are in those generated .py files. For example, if I have some_function() in some_notebook.ipynb, I add:

```python
notebook_to_python("some_notebook.ipynq", "exported_script.py")
from exported_script.py import some_function
```

:-)
To run Jupyter Notebook with Poetry's dependencies enabled, you can follow these steps:

1. First, make sure you're in your project directory where the `pyproject.toml` file is located.

2. Add Jupyter to your project dependencies:

   ```
   poetry add jupyter
   ```

3. Activate the Poetry shell:

   ```
   poetry shell
   ```

4. Once in the Poetry shell, install the Jupyter kernel for your project:

   ```
   python -m ipykernel install --user --name=pdf_processor
   ```

   Replace "pdf_processor" with a name that makes sense for your project.

5. Now, still within the Poetry shell, start Jupyter Notebook:

   ```
   jupyter notebook
   ```

6. Jupyter Notebook should open in your default web browser. When you create a new notebook, make sure to select the kernel you just created ("pdf_processor" or whatever name you chose) from the dropdown menu.

Alternatively, if you prefer to run Jupyter Notebook without activating the Poetry shell each time, you can use:

```
poetry run jupyter notebook
```

This command will start Jupyter Notebook with access to all the dependencies specified in your `pyproject.toml` file.

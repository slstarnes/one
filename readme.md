
# Callistory

`callistory` is a reusable project to assist creating DIY technology events.  This project will prototype the first Callisto Morn event in Atlanta, Georgia on November 11.

# Build

All build logic is contained with in the `readme.ipynb` file.  Use `nbconvert` to execute this notebook with the command below.

    !jupyter nbconvert --inplace --execute --to notebook readme.ipynb


```python
    !jupyter nbconvert --to markdown *.ipynb
    !jupyter nbconvert --TemplateExporter.exclude_input=True --TemplateExporter.exclude_input=True index.ipynb 
```


    !jupyter nbconvert --to markdown *.ipynb
    !jupyter nbconvert --TemplateExporter.exclude_input=True --TemplateExporter.exclude_input=True index.ipynb 


# [contributing](contributing.ipynb)


```python
    %%file custom.css
    .output code {display: none;}
```


    %%file custom.css
    .output code {display: none;}


    Overwriting custom.css


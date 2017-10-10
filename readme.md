
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
    # !jupyter nbconvert --execute --TemplateExporter.exclude_input=True --TemplateExporter.exclude_input=True index.ipynb 


    [NbConvertApp] Converting notebook about.ipynb to markdown
    [NbConvertApp] Writing 449 bytes to about.md
    [NbConvertApp] Converting notebook contributing.ipynb to markdown
    [NbConvertApp] Writing 648 bytes to contributing.md
    [NbConvertApp] Converting notebook index.ipynb to markdown
    [NbConvertApp] Writing 430 bytes to index.md
    [NbConvertApp] Converting notebook long.ipynb to markdown
    [NbConvertApp] Writing 1177 bytes to long.md
    [NbConvertApp] Converting notebook participants.ipynb to markdown
    [NbConvertApp] Writing 30 bytes to participants.md
    [NbConvertApp] Converting notebook readme.ipynb to markdown
    [NbConvertApp] Writing 951 bytes to readme.md
    [NbConvertApp] Converting notebook short.ipynb to markdown
    [NbConvertApp] Writing 124 bytes to short.md


# [contributing](contributing.ipynb)


```python
    %%file custom.css
    .output code {display: none;}
```


    %%file custom.css
    .output code {display: none;}


    Overwriting custom.css


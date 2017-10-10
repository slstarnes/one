
# Callistory

`callistory` is a reusable project to assist creating DIY technology events.  This project will prototype the first Callisto Morn event in Atlanta, Georgia on November 11.

# Build

All build logic is contained with in the `readme.ipynb` file.  Use `nbconvert` to execute this notebook with the command below.

    !jupyter nbconvert --inplace --execute --to notebook readme.ipynb
    
## [Conference Website](https://tonyfast.github.io/callistory/)


This project maintains an index of notebooks on the `master` branch.  The Github Pages deployment separates out the HTML and Markdown content from the source documents.   

### [Travis Pages Deployment](https://docs.travis-ci.com/user/deployment/pages/)


```python
    %reload_ext literacy
    !jupyter nbconvert --to markdown *.ipynb
    !jupyter nbconvert --TemplateExporter.exclude_input=True --TemplateExporter.exclude_input=True index.ipynb 
```


    %reload_ext literacy
    !jupyter nbconvert --to markdown *.ipynb
    !jupyter nbconvert --TemplateExporter.exclude_input=True --TemplateExporter.exclude_input=True index.ipynb 


    [NbConvertApp] Converting notebook about.ipynb to markdown
    [NbConvertApp] Writing 769 bytes to about.md
    [NbConvertApp] Converting notebook contributing.ipynb to markdown
    [NbConvertApp] Writing 648 bytes to contributing.md
    [NbConvertApp] Converting notebook index.ipynb to markdown
    [NbConvertApp] Writing 5577 bytes to index.md
    [NbConvertApp] Converting notebook long.ipynb to markdown
    [NbConvertApp] Writing 1157 bytes to long.md
    [NbConvertApp] Converting notebook participants.ipynb to markdown
    [NbConvertApp] Writing 30 bytes to participants.md
    [NbConvertApp] Converting notebook readme.ipynb to markdown
    [NbConvertApp] Writing 2877 bytes to readme.md
    [NbConvertApp] Converting notebook short.ipynb to markdown
    [NbConvertApp] Writing 120 bytes to short.md
    [NbConvertApp] Converting notebook index.ipynb to html
    [NbConvertApp] Writing 257988 bytes to index.html



```python
contributing.md
```



# [contributing](contributing.ipynb)

`callistory` treats DIY event organization as open source piece of software.

## Development

* __[readme.ipynb](readme.ipynb)__ provides instruction for external services.
* __[about.ipynb](about.ipynb)__ provides information about the event.  Who what where when how why.
* __[long.ipynb](long.ipynb)__ provides provides long format presentations information.
* __[short.ipynb](short.ipynb)__ provides provides short format presentations information.
* __[participants.ipynb](participants.ipynb)__ provides extra information about the conference participants.
* __[code_of_conduct.md](code_of_conduct.md)__




```python
    %%file custom.css
    .output code {display: none;}
```


    %%file custom.css
    .output code {display: none;}


    Overwriting custom.css


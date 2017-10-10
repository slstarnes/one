

```python
    %reload_ext literacy
```


```python
about.md
```

---

# Developer

All build logic is contained with in the `readme.ipynb` file.  Use `nbconvert` to execute this notebook with the command below.

    !jupyter nbconvert --to markdown --config config.py readme.ipynb
    
## [Conference Website](https://tonyfast.github.io/callistory/)


This project maintains an index of notebooks on the `master` branch.  The Github Pages deployment separates out the HTML and Markdown content from the source documents.   

### [Travis Pages Deployment](https://docs.travis-ci.com/user/deployment/pages/)


```python
    %%file config.py
    c.Exporter.preprocessors.append('literacy.template.Execute')
    c.TemplateExporter.exclude_input=True
    c.TemplateExporter.exclude_input_prompt=True
```


```python
    !jupyter nbconvert --to markdown *.ipynb
    !jupyter nbconvert --config config.py index.ipynb 
```


```python
contributing.md
```


```python
    %%file custom.css
    .output code {display: none;}
```

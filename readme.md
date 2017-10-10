

```python
    %reload_ext literacy
```


```python
about.md
```



# Callisto Morn #1

## _on_ Saturday November 11, 2017 _@_ the Georgia Tech Research Institute

__Callisto Morn__ is a satellite conference orbitting the Project Jupyter.  At each __Callisto Morn__, Jupyter beginners and veterans will join to share the gravity of their work.  These events will organize designers, developers, and scientists across the southeast region.

## [Submit a Talk](https://docs.google.com/forms/d/e/1FAIpQLSfY1c4y2vLE-q3VMBjOpvTi4pK5D6Q9KudNk25AsxQUjsT3eA/viewform)


## [Github](https://github.com/tonyfast/callistory) 

[![Gitter](https://badges.gitter.im/tonyfast/callistory.svg)](https://gitter.im/tonyfast/callistory?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=body_badge)


[![Build Status](https://travis-ci.org/tonyfast/callistory.svg?branch=master)](https://travis-ci.org/tonyfast/callistory)

---

# Coming Soon

## ~~[Tickets]()~~



---

# Developer

All build logic is contained with in the `readme.ipynb` file.  Use `nbconvert` to execute this notebook with the command below.

    !jupyter nbconvert --inplace --execute --to notebook readme.ipynb
    
## [Conference Website](https://tonyfast.github.io/callistory/)


This project maintains an index of notebooks on the `master` branch.  The Github Pages deployment separates out the HTML and Markdown content from the source documents.   

### [Travis Pages Deployment](https://docs.travis-ci.com/user/deployment/pages/)


```python
    !jupyter nbconvert --to markdown *.ipynb
    !jupyter nbconvert --TemplateExporter.exclude_input=True --TemplateExporter.exclude_input=True index.ipynb 
```


    !jupyter nbconvert --to markdown *.ipynb
    !jupyter nbconvert --TemplateExporter.exclude_input=True --TemplateExporter.exclude_input=True index.ipynb 



```python
contributing.md
```


```python
    %%file custom.css
    .output code {display: none;}
```

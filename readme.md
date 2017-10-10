


# Callisto Morn #1

## _on_ Saturday November 11, 2017 _@_ the Georgia Tech Research Institute

__Callisto Morn__ is a satellite conference orbitting the Project Jupyter.  At each __Callisto Morn__, Jupyter beginners and veterans will join to share the gravity of their work.  These events will organize designers, developers, and scientists across the southeast region.

## [Submit a Talk](https://docs.google.com/forms/d/e/1FAIpQLSfY1c4y2vLE-q3VMBjOpvTi4pK5D6Q9KudNk25AsxQUjsT3eA/viewform)


## [Github](https://github.com/tonyfast/callistory) 

[![Gitter](https://badges.gitter.im/tonyfast/callistory.svg)](https://gitter.im/tonyfast/callistory?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=body_badge)


[![Build Status](https://travis-ci.org/tonyfast/callistory.svg?branch=master)](https://travis-ci.org/tonyfast/callistory)


## [Questions?](https://github.com/tonyfast/callistory/issues) 

---

# Coming Soon

## ~~[Tickets]()~~



---

# Developer

All build logic is contained with in the `readme.ipynb` file.  Use `nbconvert` to execute this notebook with the command below.

    !jupyter nbconvert --to markdown --config config.py readme.ipynb
    
## [Conference Website](https://tonyfast.github.io/callistory/)


This project maintains an index of notebooks on the `master` branch.  The Github Pages deployment separates out the HTML and Markdown content from the source documents.   

### [Travis Pages Deployment](https://docs.travis-ci.com/user/deployment/pages/)


    %%file config.py
    c.Exporter.preprocessors.append('literacy.template.Execute')
    c.TemplateExporter.exclude_input=True
    c.TemplateExporter.exclude_input_prompt=True


    Overwriting config.py



    !jupyter nbconvert --to markdown *.ipynb
    !jupyter nbconvert --config config.py index.ipynb 


    [NbConvertApp] Converting notebook about.ipynb to markdown


    [NbConvertApp] Writing 959 bytes to about.md
    [NbConvertApp] Converting notebook contributing.ipynb to markdown
    [NbConvertApp] Writing 857 bytes to contributing.md
    [NbConvertApp] Converting notebook index.ipynb to markdown
    [NbConvertApp] Writing 5709 bytes to index.md
    [NbConvertApp] Converting notebook long.ipynb to markdown
    [NbConvertApp] Writing 1157 bytes to long.md
    [NbConvertApp] Converting notebook participants.ipynb to markdown
    [NbConvertApp] Writing 30 bytes to participants.md
    [NbConvertApp] Converting notebook readme.ipynb to markdown
    [NbConvertApp] Writing 3972 bytes to readme.md
    [NbConvertApp] Converting notebook short.ipynb to markdown
    [NbConvertApp] Writing 120 bytes to short.md


    [NbConvertApp] Converting notebook index.ipynb to html
    [NbConvertApp] Executing notebook with kernel: python3


    [NbConvertApp] Writing 258674 bytes to index.html




# [contributing](contributing.ipynb)

`callistory` treats DIY event organization as open source piece of software.

## [Submit questions and suggestions through the github issues](https://github.com/tonyfast/callistory/issues)

We hope that community participation can assist future organizers in producing diy technology events.

## Development

* __[readme.ipynb](readme.ipynb)__ provides instruction for external services.
* __[about.ipynb](about.ipynb)__ provides information about the event.  Who what where when how why.
* __[long.ipynb](long.ipynb)__ provides provides long format presentations information.
* __[short.ipynb](short.ipynb)__ provides provides short format presentations information.
* __[participants.ipynb](participants.ipynb)__ provides extra information about the conference participants.

# [Code of Conduct](code_of_conduct.md)




    %%file custom.css
    .output code {display: none;}


    Overwriting custom.css


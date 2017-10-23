

```python
    %reload_ext literacy
```


```python
about.md
```



# Callist☾ M☾rn One

## _on_ Saturday November 11, 2017 _@_ the Georgia Tech Research Institute

__Callisto Morn__ is a satellite conference orbitting the Project Jupyter.  At each __Callisto Morn__, Jupyter beginners and veterans will join to share the gravity of their work.  These events will organize designers, developers, and scientists across the southeast region.

## [Submit a Talk](https://docs.google.com/forms/d/e/1FAIpQLSfY1c4y2vLE-q3VMBjOpvTi4pK5D6Q9KudNk25AsxQUjsT3eA/viewform)


## [Github](https://github.com/callisto-morns/one) 


## [Questions?](https://github.com/callisto-morns/one/issues) 

[![Gitter chat](https://badges.gitter.im/callisto-one/Lobby.png)](https://gitter.im/callisto-one/Lobby)

---
## Announcements

{% for post in site.posts %}* [{{ post.title }}]({{ post.url }})
{% endfor %}
# Coming Soon

## ~~[Very Afforable Tickets]()~~



---

# Developer

All build logic is contained with in the `readme.ipynb` file.  Use `nbconvert` to execute this notebook with the command below.

    !jupyter nbconvert --to markdown --config config.py readme.ipynb
    
## [Conference Website](https://tonyfast.github.io/callistory/)


This project maintains an index of notebooks on the `master` branch.  The Github Pages deployment separates out the HTML and Markdown content from the source documents.   

### [Travis Pages Deployment](https://docs.travis-ci.com/user/deployment/pages/)


```python
    %%file config.py
    c.Exporter.preprocessors = ['literacy.template.Execute']
    c.TemplateExporter.exclude_input=True
    c.TemplateExporter.exclude_input_prompt=True
    
```

    Overwriting config.py



```python
    !jupyter nbconvert --to markdown *.ipynb 
    !jupyter nbconvert --to markdown --FilesWriter.build_directory=_posts posts/2017-*.ipynb 
    !echo "---\n---\n" > index.html
    !jupyter nbconvert --config config.py --stdout index.ipynb >> index.html
```

    [NbConvertApp] Converting notebook about.ipynb to markdown
    [NbConvertApp] Writing 948 bytes to about.md
    [NbConvertApp] Converting notebook announcement.ipynb to markdown
    [NbConvertApp] Writing 2276 bytes to announcement.md
    [NbConvertApp] Converting notebook contributing.ipynb to markdown
    [NbConvertApp] Writing 902 bytes to contributing.md
    [NbConvertApp] Converting notebook index.ipynb to markdown
    [NbConvertApp] Writing 3638 bytes to index.md
    [NbConvertApp] Converting notebook participants.ipynb to markdown
    [NbConvertApp] Writing 30 bytes to participants.md
    [NbConvertApp] Converting notebook readme.ipynb to markdown
    [NbConvertApp] Writing 4825 bytes to readme.md
    [NbConvertApp] Converting notebook talks.ipynb to markdown
    [NbConvertApp] Writing 2400 bytes to talks.md
    [NbConvertApp] Converting notebook posts/2017-10-23-Adding-the-first-talks.ipynb to markdown
    [NbConvertApp] Writing 779 bytes to _posts/2017-10-23-Adding-the-first-talks.md
    [NbConvertApp] Converting notebook index.ipynb to html
    [NbConvertApp] Executing notebook with kernel: python3



```python
    %%file schedule.csv
start,end,section,description
8:30,9:00,Registration,Code of Conduct
9:00,9:10,Open remarks,
9:10,9:45,Panel Discussion,4 people
9:45,10:15,30 Min Case Study,
10:15,10:45,30 Min Case Study,
10:45,11:15,Powers Often,Nick and Tony
11:15,11:30,Break,Left over coffee
11:30,11:40,10 min talk,
11:40,11:50,10 min talk,Greg Werner
11:50,12:05,15 min talk,
12:05,12:20,15 min talk,Casey Hartnett
12:20,12:30,Question from previous talks,
12:30,12:45,Tiny Talks,Shorts 2 min talks about the day
12:45,1:00,Business Business Business,Announcements
```

    Overwriting schedule.csv



```python
contributing.md
```



# [contributing](contributing.ipynb)

[![Build Status](https://travis-ci.org/tonyfast/callistory.svg?branch=master)](https://travis-ci.org/tonyfast/callistory)

## [Submit questions and suggestions through the github issues](https://github.com/tonyfast/callistory/issues)

We hope that community participation can assist future organizers in producing diy technology events.

## Development

* __[readme.ipynb](readme.ipynb)__ provides instruction for external services.
* __[about.ipynb](about.ipynb)__ provides information about the event.  Who what where when how why.
* __[long.ipynb](long.ipynb)__ provides provides long format presentations information.
* __[short.ipynb](short.ipynb)__ provides provides short format presentations information.
* __[participants.ipynb](participants.ipynb)__ provides extra information about the conference participants.

# [Code of Conduct](code_of_conduct.md)




```python
    %%file custom.css
    .output code {display: none;}
```


    %%file custom.css
    .output code {display: none;}


    Writing custom.css


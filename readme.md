

about.md


---

# Developer

All build logic is contained with in the `readme.ipynb` file.  Use `nbconvert` to execute this notebook with the command below.

    !jupyter nbconvert --to markdown --config config.py readme.ipynb
    
## [Conference Website](https://tonyfast.github.io/callistory/)


This project maintains an index of notebooks on the `master` branch.  The Github Pages deployment separates out the HTML and Markdown content from the source documents.   

### [Travis Pages Deployment](https://docs.travis-ci.com/user/deployment/pages/)


    %%file config.py
    c.TemplateExporter.exclude_input=True
    c.TemplateExporter.exclude_input_prompt=True


    Overwriting config.py



    !jupyter nbconvert --to markdown *.ipynb 
    !jupyter nbconvert --to markdown --FilesWriter.build_directory=_posts posts/2017-*.ipynb 
    #     !rm index.md
    !echo "---\n---\n" > index.html
    !jupyter nbconvert --config config.py --stdout index.ipynb >> index.html
    !jupyter nbconvert --config config.py --to markdown readme.ipynb


    [NbConvertApp] Converting notebook about.ipynb to markdown
    [NbConvertApp] Writing 1366 bytes to about.md
    [NbConvertApp] Converting notebook announcement.ipynb to markdown
    [NbConvertApp] Writing 2276 bytes to announcement.md
    [NbConvertApp] Converting notebook contributing.ipynb to markdown
    [NbConvertApp] Writing 864 bytes to contributing.md
    [NbConvertApp] Converting notebook demonstrations.ipynb to markdown
    [NbConvertApp] Writing 4028 bytes to demonstrations.md
    [NbConvertApp] Converting notebook index.ipynb to markdown
    [NbConvertApp] Writing 8994 bytes to index.md
    [NbConvertApp] Converting notebook readme.ipynb to markdown
    [NbConvertApp] Writing 6818 bytes to readme.md
    [NbConvertApp] Converting notebook posts/2017-10-23-Adding-the-first-talks.ipynb to markdown
    [NbConvertApp] Writing 784 bytes to _posts/2017-10-23-Adding-the-first-talks.md
    [NbConvertApp] Converting notebook index.ipynb to html
    [NbConvertApp] Converting notebook readme.ipynb to markdown
    [NbConvertApp] Writing 5434 bytes to readme.md



    %%file schedule.csv
    start,end,section,description
    8:30,9:00,Registration,Code of Conduct
    9:00,9:10,Open remarks,
    9:10,9:45,Panel Discussion,4 people
    9:45,10:15,30 Min Case Study, Jupyter Lab Walk Through
    10:15,10:45,30 Min Case Study, Luke Starnes
    10:45,11:15,Powers Often, Nick and Tony
    11:15,11:30,Break,Left over coffee
    11:30,12:05,25 min talk,Rajeswari Sivakumar & Christian McDaniel from Dr. Shannon Quinn's group @UGA
    11:40,11:50,10 min talk,Greg Werner
    12:05,12:20,15 min talk,Casey Hartnett
    12:20,12:30,Question from previous talks,
    12:30,12:45,Tiny Talks,Shorts 2 min talks about the day
    12:45,1:00,Business Business Business,Announcements


    Overwriting schedule.csv




# [contributing](contributing.ipynb)

[![Build Status](https://travis-ci.org/callisto-morns/one.svg?branch=master)](https://travis-ci.org/callisto-morns/one)

## [Submit questions and suggestions through the github issues](https://github.com/tonyfast/callistory/issues)

We hope that community participation can assist future organizers in producing diy technology events.

## Development

* __[readme.ipynb](readme.ipynb)__ provides instruction for external services.
* __[index.ipynb](readme.ipynb)__ the main event site.
* __[about.ipynb](about.ipynb)__ provides information about the event.  Who what where when how why.
* __[contributing.ipynb](about.ipynb)__ provides information about the event.  Who what where when how why.
* __[talks.ipynb](long.ipynb)__ provides provides long format presentations information.

# [Code of Conduct](code_of_conduct.md)




    %%file custom.css
    .output code {display: none;}


    Writing custom.css


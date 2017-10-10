
# Callistory

`callistory` is a reusable project to assist creating DIY technology events.  This project will prototype the first Callisto Morn event in Atlanta, Georgia on November 11.

# Build

All build logic is contained with in the `readme.ipynb` file.  Use `nbconvert` to execute this notebook with the command below.

    !jupyter nbconvert --inplace --execute --to notebook readme.ipynb


```python
    !jupyter nbconvert --to markdown *.ipynb
    !jupyter nbconvert --execute --TemplateExporter.exclude_input=True --TemplateExporter.exclude_input=True index.ipynb 
```


    !jupyter nbconvert --to markdown *.ipynb
    !jupyter nbconvert --execute --TemplateExporter.exclude_input=True --TemplateExporter.exclude_input=True index.ipynb 


    [NbConvertApp] Converting notebook about.ipynb to markdown
    [NbConvertApp] Writing 449 bytes to about.md
    [NbConvertApp] Converting notebook contributing.ipynb to markdown
    [NbConvertApp] Writing 648 bytes to contributing.md
    [NbConvertApp] Converting notebook index.ipynb to markdown
    [NbConvertApp] Writing 6934 bytes to index.md
    [NbConvertApp] Converting notebook long.ipynb to markdown
    [NbConvertApp] Writing 1177 bytes to long.md
    [NbConvertApp] Converting notebook participants.ipynb to markdown
    [NbConvertApp] Writing 30 bytes to participants.md
    [NbConvertApp] Converting notebook readme.ipynb to markdown
    [NbConvertApp] Writing 3112 bytes to readme.md
    [NbConvertApp] Converting notebook short.ipynb to markdown
    [NbConvertApp] Writing 124 bytes to short.md
    [NbConvertApp] Converting notebook index.ipynb to html
    [NbConvertApp] Executing notebook with kernel: python3
    [IPKernelApp] ERROR | Exception in message handler:
    Traceback (most recent call last):
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/ipykernel/kernelbase.py", line 235, in dispatch_shell
        handler(stream, idents, msg)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/ipykernel/kernelbase.py", line 399, in execute_request
        user_expressions, allow_stdin)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/ipykernel/ipkernel.py", line 196, in do_execute
        res = shell.run_cell(code, store_history=store_history, silent=silent)
      File "/Users/tonyfast/literacy2/literacy/run.ipynb", line 19, in _run_cell
        "execution_count": 7,
      File "/Users/tonyfast/anaconda/lib/python3.5/contextlib.py", line 59, in __enter__
        return next(self.gen)
      File "/Users/tonyfast/literacy2/literacy/run.ipynb", line 31, in _run
        ]
      File "/Users/tonyfast/literacy2/literacy/template.ipynb", line 47, in template
        "cell_type": "code",
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/jinja2/environment.py", line 1008, in render
        return self.environment.handle_exception(exc_info, True)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/jinja2/environment.py", line 780, in handle_exception
        reraise(exc_type, exc_value, tb)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/jinja2/_compat.py", line 37, in reraise
        raise value.with_traceback(tb)
      File "<template>", line 3, in top-level template code
    jinja2.exceptions.UndefinedError: 'presentations' is undefined
    [NbConvertApp] ERROR | Timeout waiting for execute reply (30s).
    Traceback (most recent call last):
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/preprocessors/execute.py", line 314, in run_cell
        msg = self.kc.shell_channel.get_msg(timeout=timeout)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/jupyter_client/blocking/channels.py", line 57, in get_msg
        raise Empty
    queue.Empty
    
    During handling of the above exception, another exception occurred:
    
    Traceback (most recent call last):
      File "/Users/tonyfast/anaconda/bin/jupyter-nbconvert", line 11, in <module>
        load_entry_point('nbconvert', 'console_scripts', 'jupyter-nbconvert')()
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/jupyter_core/application.py", line 267, in launch_instance
        return super(JupyterApp, cls).launch_instance(argv=argv, **kwargs)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/traitlets/config/application.py", line 658, in launch_instance
        app.start()
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/nbconvertapp.py", line 313, in start
        self.convert_notebooks()
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/nbconvertapp.py", line 481, in convert_notebooks
        self.convert_single_notebook(notebook_filename)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/nbconvertapp.py", line 452, in convert_single_notebook
        output, resources = self.export_single_notebook(notebook_filename, resources, input_buffer=input_buffer)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/nbconvertapp.py", line 381, in export_single_notebook
        output, resources = self.exporter.from_filename(notebook_filename, resources=resources)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/exporters/exporter.py", line 172, in from_filename
        return self.from_file(f, resources=resources, **kw)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/exporters/exporter.py", line 190, in from_file
        return self.from_notebook_node(nbformat.read(file_stream, as_version=4), resources=resources, **kw)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/exporters/html.py", line 84, in from_notebook_node
        return super(HTMLExporter, self).from_notebook_node(nb, resources, **kw)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/exporters/templateexporter.py", line 268, in from_notebook_node
        nb_copy, resources = super(TemplateExporter, self).from_notebook_node(nb, resources, **kw)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/exporters/exporter.py", line 132, in from_notebook_node
        nb_copy, resources = self._preprocess(nb_copy, resources)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/exporters/exporter.py", line 309, in _preprocess
        nbc, resc = preprocessor(nbc, resc)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/preprocessors/base.py", line 47, in __call__
        return self.preprocess(nb,resources)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/preprocessors/execute.py", line 242, in preprocess
        nb, resources = super(ExecutePreprocessor, self).preprocess(nb, resources)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/preprocessors/base.py", line 70, in preprocess
        nb.cells[index], resources = self.preprocess_cell(cell, resources, index)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/preprocessors/execute.py", line 260, in preprocess_cell
        outputs = self.run_cell(cell, cell_index)
      File "/Users/tonyfast/anaconda/lib/python3.5/site-packages/nbconvert/preprocessors/execute.py", line 327, in run_cell
        raise exception("Cell execution timed out")
    TimeoutError: Cell execution timed out



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


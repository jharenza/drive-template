# Cookiecutter Data Science

_A logical, reasonably standardized, but flexible project structure for doing and sharing data science work._


#### [Project homepage](http://drivendata.github.io/cookiecutter-data-science/)


### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.5
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
------------

    cookiecutter https://github.com/samesense/drive-template/

### The resulting directory structure
------------

The directory structure of your lab looks like this: 

```
/mnt/isilon/lab_drive/
├── README.md
├── archive
│   ├── README.md
│   ├── arcus
│   └── project-name-1.tar.gz
├── data
│   └── README.md
├── misc
│   └── README.md
├── projects
│   ├── README.md
│   ├── project-name-1
│   └── project-name-2
├── tools
│   ├── README.md
│   ├── bin
│   ├── include
│   ├── lib
│   ├── opt
│   ├── scif
│   │   └── softwareName__vVersion
│   │       ├── bin
│   │       ├── lib
│   │       └── scif
│   └── src
└── users
    ├── README.md
    └── evansj
        ├── README.md
        └── tmp
```

## Contributing

We welcome contributions! [See the docs for guidelines](https://drivendata.github.io/cookiecutter-data-science/#contributing).

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests

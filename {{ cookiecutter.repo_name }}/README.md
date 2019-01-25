{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

Drive Organization
------------
```
├── README.md
├── apps
│   ├── README.md
│   ├── bin
│   ├── include
│   ├── lib
│   ├── opt
│   ├── src
│   └── versioned_apps
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
└── users
    ├── README.md
    └── evansj
        └── tmp
```

--------

<p><small>Drive based on the <a target="_blank" href="github.com/samesense/drive-template/">cookiecutter drive template version 1</a>. #cookiecutterdatascience</small></p>

### organization
* apps/ holds tools/programs used by the lab that are not found in respublica modules. It's structure is based on the [Filesystem Hierarchy Standard](https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard). /mnt/isilon/dbhi_bfx/ contains many tools. Check that this directory before installing tools in apps/.
* archive/ holds old projects in tar.gz form, and arcus data
* misc/ holds everything that did not belong elsewhere
* projects/ holds all lab projects. Ideally, each project should be linked to a versioned controlled repository. When one datasset is shared between multiple projects/repositories, create a top-level directory to hold the data, and put the repos inside.
* data/ holds reference data or datasets that span multiple projects. Check /reference_data/ before adding data here.
* users/ is a free space for lab members to store files that to not fit elsewhere.

* nfs vs smb and real meaning for sharing/permissions

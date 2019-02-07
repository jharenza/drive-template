{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

This is an {{nfs.or.smb}} drive. NFS scheme allows for individual folder control of permissions, because group has write, you can make your own dir then chmod it 700 to lock out anyone else. For SMB scheme, group is created for the share and anyone in the group has rwx access to everything. No custom control of subdirectories.

Drive Organization
------------
```
/mnt/isilon/PI_drive
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
    └── evansj
        ├── README.md
        └── tmp
```

--------

<p><small>Drive based on the <a target="_blank" href="github.com/samesense/drive-template/">cookiecutter drive template version 1</a>. </small></p>

### organization
* tools/ holds tools/programs used by the lab that are not found in respublica modules. Its structure is based on the [Filesystem Hierarchy Standard](https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard). /mnt/isilon/dbhi_bfx/ contains many tools. Check that this directory before installing tools in tools/.
* archive/ holds old projects in tar.gz form, and arcus data
* misc/ holds everything that did not belong elsewhere
* projects/ holds all lab projects. Ideally, each project should be linked to a versioned controlled repository. When one datasset is shared between multiple projects/repositories, create a top-level directory to hold the data, and put the repos inside.
* data/ holds reference data or datasets that span multiple projects. Check /reference_data/ before adding data here.
* users/ is a free space for lab members to store files that to not fit elsewhere.

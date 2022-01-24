## 3.10 Reproduce a folder structure

You’re starting a new experiment and would like to duplicate the directory structure from your previous experiment so you can add new data.

Assume that the previous experiment is in a folder called ```2016-05-18```, which contains a ```data``` folder that in turn contains folders named ```raw``` and ```processed``` that contain data files. The goal is to copy the folder structure of the ```2016-05-18``` folder into a folder called ```2016-05-20``` so that your final directory structure looks like this:

```output
2016-05-20/
└── data
├── processed
└── raw
```

Which of the following set of commands would achieve this objective? What would the other commands do?

```bash
$ mkdir 2016-05-20
$ mkdir 2016-05-20/data
$ mkdir 2016-05-20/data/processed
$ mkdir 2016-05-20/data/raw
```
```bash
$ mkdir 2016-05-20
$ cd 2016-05-20
$ mkdir data
$ cd data
$ mkdir raw processed
```
```bash
$ mkdir 2016-05-20/data/raw
$ mkdir 2016-05-20/data/processed
```
```bash
$ mkdir -p 2016-05-20/data/raw
$ mkdir -p 2016-05-20/data/processed
```
```bash
$ mkdir 2016-05-20
$ cd 2016-05-20
$ mkdir data
$ mkdir raw processed
```

<details>
  <summary>
Solution
  </summary>

The first two sets of commands achieve this objective. The first set uses relative paths to create the top-level directory before the subdirectories.

The third set of commands will give an error because the default behavior of ```mkdir``` won’t create a subdirectory of a non-existent directory: the intermediate level folders must be created first.

The fourth set of commands achieve this objective. Remember, the ```-p``` option, followed by a path of one or more directories, will cause ```mkdir``` to create any intermediate subdirectories as required.

The final set of commands generates the ‘raw’ and ‘processed’ directories at the same level as the ‘data’ directory.

</details>

[Episode 4 Exercise 1](episode4_ex1.md)

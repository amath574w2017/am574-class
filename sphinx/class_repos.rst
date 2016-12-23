
.. _class_repos:

Class GitHub Repository
=======================

All of the files that you may need to access for this class will be pushed
to the GitHub repository `amath574w2017/am574-class 
<https://github.com/amath574w2017/am574-class>`_.

To clone this repository::

    git clone https://github.com/amath574w2017/am574-class.git

This will create a directory `am574-class`.  

AM574 environment variable
--------------------------

I suggest you define an environment variable `AM574` that points to this
repository, e.g. in the bash shell::

    export AM574=/full/path/to/am574-class

(You will need to adjust this to set the path properly.)

You can put this command in the file `~/.bashrc` if you want it to be
executed every time you open a new shell.  

Then you can do, e.g. ::

    cd $AM574

to change directories to the class repository.

Below and elsewhere in these notes, `$AM574` will be used to refer to the
full path to the class repository.

To update
---------

If new files have been added to the class repository, you can get them by
doing::

    cd $AM574
    git pull

Your copy of these files
------------------------

To avoid having to worry about
conflicts if you change a file and the same file changes in the repository,
I suggest that you never modify the files in this directory.  Instead, 
create another directory for doing your own work, e.g. ::

    cd
    mkdir my574
    export MY574=/full/path/to/my574

Then copy any files you need to this directory before working with them, e.g. ::

    cp -r $AM574/homeworks/hw1  $MY574/

will recursively copy the directory `hw1`.

Then modify the files in the new `hw1` directory.

Stayed tuned for instructions on pushing your results back to GitHub.



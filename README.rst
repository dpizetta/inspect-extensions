Inspect Extensions
==================

Extending Python `inspect` module to users and developers to get information
about packages, modules, classes and other members. Working on Python 3.8+.


Installing, updating and uninstalling
#####################################


To install and/or update, do ::

    $ pip install -U inspect-extensions


To remove ::

    $ pip uninstall inspect-extensions


Running
#######


To get a minimalist output ::

    $ inspect-extensions


Examples from v0.1
##################


Help
----


.. code-block:: console

    $ inspect-extensions --help


.. code-block:: console

    usage: inspect_extensions.py [-h]
        [--colored COLORED] [--filter FILTER]
        [-p PACKAGES] [-m MODULES]
        [-c CLASSES] [-t METHODS] [-f FUNCTIONS] [-d DATA]
        [-a ALL_MEMBERS]
        [-b PUBLIC] [-o PROTECTED] [-i PRIVATE]
        [--encapsulation ENCAPSULATION] [-e ALL_ENCAPSULATION]
        [--count_members COUNT_MEMBERS] [--text_only TEXT_ONLY]
        [--special_classes SPECIAL_CLASSES]
        [--special_methods SPECIAL_METHODS]
        [--special_data SPECIAL_DATA]
        [--remove_special_classes REMOVE_SPECIAL_CLASSES]
        [--remove_special_methods REMOVE_SPECIAL_METHODS]
        [--remove_special_data REMOVE_SPECIAL_DATA]
        [--remove_special_members REMOVE_SPECIAL_MEMBERS]
        obj

    Inspect Extensions module.

    Python script that uses many modules from Python to exposes
    as many information that is possible to inspect packages.

    positional arguments:

    obj                   Input object (package, module, class)

    optional arguments:

    -h, --help            Show this help message and exit
    --count_members       Shows the number of members
    --colored             Print colored members
    --text_only           Print just text characters - not colorized

    --filter FILTER       [PACKAGE, MODULE, CLASS, METHOD, DATA, ALL]

    -p PACKAGES, --packages PACKAGES
        Show just packages
    -m MODULES, --modules MODULES
        Show just modules
    -c CLASSES, --classes CLASSES
        Show just classes
    -t METHODS, --methods METHODS
        Show just methods, must have 'self' as first arg
    -f FUNCTIONS, --functions FUNCTIONS
        Show just functions, not associated with any object
    -d DATA, --data DATA
        Show just data, variables
    -a ALL_MEMBERS, --all_members ALL_MEMBERS
        Show all members (DEFAULT)(packages, modules, classes, methods, functions, data)

    --encapsulation ENCAPSULATION [NONE, PUBLIC, PROTECTED, PRIVATE, ALL]

    -b PUBLIC, --public PUBLIC
        Show just public members (DEFAULT)
    -o PROTECTED, --protected PROTECTED
        Show just protected members
    -i PRIVATE, --private PRIVATE
        Show just private members
    -e ALL_ENCAPSULATION, --all_encapsulation ALL_ENCAPSULATION
        Show all encapsulation

    --special_classes SPECIAL_CLASSES
        Print special classes, '__' before and after name
    --special_methods SPECIAL_METHODS
        Print special methods, '__' before and after name
    --special_data SPECIAL_DATA
        Print special data, '__' before and after name

    --remove_special_classes REMOVE_SPECIAL_CLASSES
        Filter special classes, see special_classes
    --remove_special_methods REMOVE_SPECIAL_METHODS
        Filter special methods, see special_methods
    --remove_special_data REMOVE_SPECIAL_DATA
        Filter special data, see special_data
    --remove_special_members REMOVE_SPECIAL_MEMBERS
        Filter special members, see special_members

    --version
        Show program's version number and exit

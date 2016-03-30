=======================================================
reqlice
=======================================================

Annotate your requirements with the license of each requirement.
Prints the updated requirements file to stdout. Pipe it as you see fit.
At the moment it can only read requirements in the form :code:`package==version`, no :code:`>` or :code:`,` etc.

------------
Installation
------------

.. code-block:: bash

    pip install reqlice

-----
Usage
-----

To stdout:

.. code-block:: bash

    $ reqlice requirements.txt
    Babel==1.3                        # BSD License
    billiard==3.3.0.20                # BSD License
    celery==3.1.23                    # BSD License

Pipe to file:

.. code-block:: bash

    $ reqlice requirements.txt 1> updated_requirements.txt
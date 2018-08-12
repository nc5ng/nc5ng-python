Installation
============

Installation instructions for nc5ng-python


System Installation
-------------------

``nc5ng`` offers common installation options for python distributions

.. note::

   It is recommended to use a python virtual environment (``virtualenv``) to install this package and dependencies.
   Installing directly to a system python distribution can break certain system packages.

Requirements
~~~~~~~~~~~~
   
- Python 3.x
  - ``pip`` and ``virtualenv`` (`Recommended`)
- Fortran (``gfortran``)
- GMT (4.x-6.x)
- GMT/Python (`Optional`)
  - GMT6.0 Required for ``GMT/Python``(`Development Release Only`)

Python Package Index
~~~~~~~~~~~~~~~~~~~~

Released versions of ``nc5ng`` can be installed directly from the PyPi by using  `pip` 
::

   pip install nc5ng


Specific versions can be installed by specifying ``nc5ng==VERSION``


Development Versions
~~~~~~~~~~~~~~~~~~~~

``pip`` can be used to install development versions of python packages by
specifying the git repository, including branch or commit
::
   
   pip install -U git+git://github.com/nc5ng/nc5ng-python@stable
   pip install -U git+git://github.com/nc5ng/nc5ng-python@8f482ba1ce6484ab18e6ccd88d6e251655cd61f2



Local Copies can be installed in editable mode for development
::
   git clone git@github.com/nc5ng/nc5ng-python
   pip install -U -e ./nc5ng-python




Docker Deployment
-----------------

Docker images are provided to use nc5ng through container virtualization. 

Pre-configured images are available from the  `nc5ng-docker <https://www.nc5ng.org/projects/nc5ng-docker>`_ project (`Dockerhub <https://hub.docker.com/r/nc5ng/nc5ng>`_), and base images with gmt tools are available from the `gmt-docker <https://www.nc5ng.org/projects/gmt-docker>`_ project (`Dockerhub <https://hub.docker.com/r/nc5ng/gmt>`_).

For convenience, the docker image ``nc5ng/nc5ng`` contains a pre-compiled conversion for testing.

For more information on deployment and use please see the docker project pages.




Requirements
~~~~~~~~~~~~
- ``docker``
- ``docker-compose`` (`Optional`)

  


.. _s-install-conversion:
  
Install Conversion Data
-----------------------


Raw Source data is provided directly from the `nc5ng-core` package. However conversion data must either be built or downloaded seperately.


Conversion data are released publically on the `nadcon5-ng github <https://github.com/nc5ng/nadcon5-ng/releases>`_ or upstream via National Geodetic Survey. For compilation please see the source library `docs <https://docs.nc5ng.org/latest>`_ , `project homepage <https://www.nc5ng.org/project/nadcon5-ng>`_, and `github <https://github.com/nc5ng/nadcon5-ng>`_


Conversion data can be placed anywhere and is referenced by configration arguments used to load data.

Installation
============

Installation instructions for generic packages

Requirements
------------

- Fortran (``f77``, ``gfortran``)
- GMT/Python (Optional)
  - GMT6.0 (Unreleased)    
  

`pip`
-----

``nc5ng`` can be installed directly through `pip` simply by running

``pip install nc5ng``




`Docker`
--------

Docker images are provided to evaluate nc5ng. Pre-configured images are available from the  `nc5ng-docker <https://www.nc5ng.org/projects/nc5ng-docker>`_ project (`Dockerhub <https://hub.docker.com/r/nc5ng/nc5ng>`_), and base images with gmt tools are available from the `gmt-docker <https://www.nc5ng.org/projects/gmt-docker>`_ project (`Dockerhub <https://hub.docker.com/r/nc5ng/gmt>`_)

`NADCON5.0` Conversion Data
---------------------------

Source data is provided directly from the `nc5ng-core` package. However conversion data must either be built or downloaded seperately.


Conversion data are released publically on the `nadcon5-ng github <https://github.com/nc5ng/nadcon5-ng/releases>`_ or upstream via National Geodetic Survey. For compilation please see the source library `docs <https://docs.nc5ng.org/latest>`_ , `project homepage <https://www.nc5ng.org/project/nadcon5-ng>`_, and `github <https://github.com/nc5ng/nadcon5-ng>`_


Conversion data can be placed anywhere and is referenced by configration arguments used to load data.
